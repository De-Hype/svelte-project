<script>
  let PricingData = [
    {
      id: 1,
      name: "Free Trial",
      price: 0,
      feature_one: "Access to account dashboard",
      feature_two: "Access to finance literacy materials",
      feature_three: "24/7 email and customer support",
      feature_four: "",
      feature_five: "",
    },
    {
      id: 2,
      name: "Starter",
      price: 10.99,
      feature_one: "Access to account dashboard",
      feature_two: "Access to finance literacy materials",
      feature_three: "24/7 email and customer support",
      feature_four: "Indepth expense report",

      feature_five: "",
    },
    {
      id: 3,
      name: "Pro",
      price: 19.99,
      feature_one: "Access to account dashboard",
      feature_two: "Access to finance literacy materials",
      feature_three: "24/7 email and customer support",
      feature_four: "Indepth expense report",
      feature_five: "Access to intergrate with third party API tools",
    },
  ];
</script>

<pricing>
  <div class="container">
    {#each PricingData as plans (plans.id)}
      <div class="card">
        <h4>{plans.name}</h4>
        <h3 class="">${plans.price}</h3>
        <div class="">
          <ul>
            <li>{plans.feature_one}</li>
            <li>{plans.feature_two}</li>
            <li>{plans.feature_three}</li>
            <li>{plans.feature_four}</li>
            <li>{plans.feature_five}</li>
          </ul>
        </div>
        <button>Subscribe</button>
      </div>
    {/each}
  </div>
</pricing>

<style>
  .container {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    padding: 0.9rem 1.2rem;
    gap: 0.9rem;
    border: 1px solid red;
    min-height: 400px;
  }
  .card {
    display: flex;
    gap: 0.6rem;
    align-items: center;
    /* justify-content: center; */
    flex-direction: column;
    padding: 0.9rem 1.2rem;
    background-color: rgb(129, 129, 243);
    height: 100%;
    position: relative;
  }
  h3 {
    font-size: 2.3rem;
    color: white;
  }
  ul{
    list-style: none;
    display: flex;
    flex-direction: column;
    gap: 1.3rem;
    padding-top: .9rem;
  }
  button {
    width: 80%;
    border: none;
    outline: none;
    padding: 0.4rem;
    font-weight: 800;
    background-color: white;
    color: blue;
    position: absolute;
    bottom: 1.4rem;
  }
</style>

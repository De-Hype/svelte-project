<script>
  import logo from "../../assets/svelte.svg";
</script>

<footer>
  <div class="footer-col-one">
    <img src={logo} alt="" />
    <p>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Excepturi in nisi
      ipsum, accusantium a, maxime cupiditate, incidunt repellendus fugit fugiat
      id eos eius alias quibusdam neque.
    </p>
  </div>
  <div class="footer-col-two">
    <h4>Product</h4>
    <div class="footer-navigations">
        <p>Home</p>
        <p>Pricing</p>
        <p>Testimony</p>
        <p class="wrapper">Careers <span>Hiring</span></p>
    </div>
  </div>
  <div class="footer-col-two">
    <h4>Product</h4>
    <div class="footer-navigations">
        <p>Home</p>
        <p>Pricing</p>
        <p>Testimony</p>
        <p>Careers </p>
    </div>
  </div>
</footer>

<style>
    footer{
        display:grid;
        grid-template-columns: repeat(3, 1fr);
        padding: 1.2rem;
        gap: 2rem;
    }
    .footer-col-two, .footer-navigations{
        display: flex;
        flex-direction: column;
        gap: .8rem;
    }
    footer-col-two h4{
      font-size: .8rem;
        font-weight: 800;
    }
    .footer-navigations p{
        font-size: .91rem;
        font-weight: 700;
        cursor:pointer;
    }
    .wrapper{
        display: flex;
        gap: .5rem;
        align-items: center;
    }
    span{
        background-color: black;
        color: white;
        font-size: .80rem;
        padding: 3px;
        border-radius: 30%;
    }
</style>

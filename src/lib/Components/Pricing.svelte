<script>
    let PricingData = [
        {
            'id':1,
            'name':'Free Trial',
            'price':10,
            // 'features':{
            //     'id':1,

            // },
        },
        {
            'id':2,
            'name':'Starter',
            'price':10,
            // 'features':{
            //     'id':1,

            // },
        },
        {
            'id':3,
            'name':'Pro',
            'price':16,
            // 'features':{
            //     'id':1,

            // },
        },
    ]
</script>
<pricing>
    <div class="container">
        {#each PricingData as plans (plans.id)}
        <div class="card">
            <h3 class="">${plans.price}</h3>
            <button>{plans.name}</button>
        </div>
    {/each}
    </div>
</pricing>

<style>
    .container{
        display: grid;
        grid-template-columns: repeat(3, 1fr);
    }
    .card{
        border: 1px solid red;
        display: flex;
        align-items:center;
        justify-content: center;
        flex-direction: column;
    }
</style>
<template>
    <section class="numbers container-fluid">
        <div class="container">
            <div class="row">
                <div class="col-12 text-center heading">
                    <h5>See our numbers</h5>
                </div>
            </div>
            <div class="number__wrapper">
                <div class="number__card text-center">
                    <i class="fa fa-users number-icons"></i>
                    <h5>2,000+</h5>
                    <p>Farmers</p>
                </div>
                <div class="number__card text-center">
                    <i class="fa fa-money number-icons"></i>
                    <h5>&#8358; 500,000+</h5>
                    <p>Invested</p>
                </div>
                <div class="number__card text-center">
                    <i class="fa fa-cubes number-icons"></i>
                    <h5>10,000+</h5>
                    <p>Acres Available</p>
                </div>
                <div class="number__card text-center">
                    <i class="fa fa-comments number-icons"></i>
                    <h5>10+</h5>
                    <p>Media Mentions</p>
                </div>
                <div class="number__card text-center">
                    <i class="fa fa-user-plus number-icons"></i>
                    <h5>10</h5>
                    <p>Team Members</p>
                </div>
            </div>
        </div>
    </section>
</template>
<script>
export default {
    name: 'CurrentNumbers'
}
</script>
<style lang="scss" scoped>
@import '../styles/colors';
.numbers{
    background: $primary-color;
    padding:3rem 0;
    .heading{
        font-family: 'Roboto';
        color:#fff;
        font-size: 1rem;
        text-transform: capitalize;
        // padding-top: 3rem;
        padding-bottom: 1rem;
    }
    .number__wrapper{
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
        grid-gap: 20px;
        .number__card{
            background:#fff;
            border-radius: 3px;
            padding: 1rem;
            border:2px solid #f4f4f4;
            border-radius: 4px;
            font-family: 'Lato';
            margin-bottom: .4rem;
            .number-icons{
                color:$primary-color;
                font-size: 1.4rem;
                padding-bottom: .4rem;
            }
            h5{
                font-weight: bold;
                font-size: 1rem;
                color:#3c3c3c;
            }
            p{
                color:#627081;
            }
        }
    }
}
</style>
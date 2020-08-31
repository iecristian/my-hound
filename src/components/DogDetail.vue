<template>
    <div class="dog-info">
        <div class="offer-date">Thursday 3 Sep 2020 - 15:10</div>
        <img src="../assets/lab.png">
        <div class="dog-feature">
            <span class="breed-name">Labrador</span>
            <span class="year">2019</span>
        </div>
        <div class="dog-feature">
            <span class="view-count">7,732 Views</span>
        </div>
        <div class=" dog-feature dog-location">
            <label class="subtitle">Location</label>
            <br>
            <label>Riyadh Yard, Saudi Arabia</label>
        </div>
        <div class="dog-feature">
            <span class="dog-price">
                <label class="subtitle">Sold for</label>
                <label>23,911</label>
                <label>SAR</label>
            </span>
            
            <span class="highest-offer">
                <label class="subtitle">Buy now</label>
                <label>23,911</label>
                <label>SAR</label>
            </span>
        </div>
        <div class="bids">View 3 Bids</div>
    </div>

</template>

<script>
export default {
    name: 'DogDetail',
    props:{
        
    }
}
</script>

<style scoped>
.dog-info{
    width: 18%; 
    position: relative;   
    float:right;
    margin: 10px;
    padding: 10px;
    min-width: 250px;
    overflow:hidden;
    background-color: #FFFFFF;
}

.dog-feature{
    padding: 0px 5px 0px 5px;
    border-bottom: 1px solid #EBEBEB; 
}

.offer-date{
    background: linear-gradient(to right, #B94646, #E73054);
    /*background-color: #E73054;*/
    color:white;
    border-radius: 3px;
    padding: 5px;
    margin-bottom: 5px;
}

img{
    border-radius: 0px 0px 20px 20px;
    width: 100%;
}

span{
    clear: both;    
}

.breed-name
{
    font-size: 2em;
     
    position: relative;
    float: left;  
}

.year{
    position: relative;
    
}

.view-count{
    border-bottom: 1px solid #EBEBEB;    
}

.dog-location{
    border-bottom: 1px solid #EBEBEB;  
    background-image: url("../assets/pin (3).svg");
    background-repeat: no-repeat;  
}

.subtitle{
    color:#989898
}

.bids{
    background: linear-gradient(to right, #74B946, #8FB946);
    /*background-color: #E73054;*/
    color:white;
    border-radius: 3px;
    padding: 5px;
    margin-bottom: 5px;
}

@media screen and (max-width: 600px) {

    .dog-info{
        width: 100%; 
        margin-left:auto;
        margin-right:auto;
    }

}

</style>
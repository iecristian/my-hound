<template>
    <div class="filters">
        <!--<div class="dropdown">
            <button class="dropdown-btn">Size</button>
            <div class="dropdown-content"> 
                <span>Small</span>
                <span>Medium</span>
                <span>Big</span>
            </div>
        </diV>-->
        <select name="age" class="filter-select">
            <option value="">Size</option>
            <option value="s">Small</option>
            <option value="m">Medium</option>
            <option value="b">Big</option>
        </select>
        <br>
         <select name="age" class="filter-select">
            <option value="">Age</option>
            <option value="1">1</option>
            <option value="2">2</option>
            <option value="3">3</option>
        </select>
        <br>
        <select name="city" class="filter-select">
            <option value="">City</option>
            <option value="bos">Boston</option>
            <option value="hou">Houston</option>
            <option value="mia">Miami</option>
        </select>
        <select name="city" class="filter-select half-width">
            <option value="">From</option>
            <option value="bos">Boston</option>
            <option value="hou">Houston</option>
            <option value="mia">Miami</option>
        </select>
        <select name="city" class="filter-select half-width">
            <option value="">To</option>
            <option value="bos">Boston</option>
            <option value="hou">Houston</option>
            <option value="mia">Miami</option>
        </select>
        <input type="text" class="filter-input" placeholder="Plate ID">
        <label class="filter-label" for="">Budget</label>
        <input type="range" min="1" max="5000" value="0" class="slider" id="priceRange1">
        <input type="range" min="5000" max="10000" value="10000" class="slider" id="priceRange2">
        <label class="minRange" for="">$0</label>
        <label class="maxRange" for="">$10,000+</label>
        <button class="search-button"><img src="../assets/search-white.svg">SEARCH</button>
    </div>
</template>

<script>
// size, age, city, from, to
export default {
    name: 'Filters',
    props:{
        
    }
}
</script>

<style scoped>
    .filters{
        width: 15%;
        float: left;
        min-width: 235px;
        border: 1px solid #44444414;
        overflow: hidden;
        padding: 5px;
        background-color: #FFFFFF;
        margin-top: 10px;
    }

    @media screen and (max-width: 600px) {

    .filters{
        display: none;
    }

}

    .filter-select, .filter-input, .filter-label{
        width: 80%;
        height: 30px;
        text-align: left;
        border:none;
        border-bottom: 1px solid #EBEBEB;
        margin: 10px;
        font-size: 0.8em;
        color: #22232B;
    }

    .filter-label{
        border: none;
        margin-bottom: 0px;
        padding: 0;
    }

    .half-width {
        width: 40%;
        margin-left: 5px;
        margin-right: 5px;
    }

    .filter-input::placeholder{
        color:#22232B;
    }

    .filter-input:focus{
        outline:none;
         border-bottom: 1px solid #22232B;
    }

    .dropdown{
        margin-bottom: 10px;
    }

    .dropdown-btn{
        height: 32px;
        width: 100%;
        background-color: #FFFFFF;
        border: none;
        text-align: left;
        border-bottom: 1px solid #EBEBEB; 
    }

    .dropdown-content{
        display: none;
        /*position: absolute;*/
        background-color: #f9f9f9;
        min-width: 160px;
        box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
        z-index: 1;
    }

    .dropdown:hover > .dropdown-content {
        display: block;
    }

    .dropdown-content > span {
        width: 100%;    
    }

    .slider {
        -webkit-appearance: none;
        width: 50%;
        height: 1px;
        background: #EBEBEB;
        outline: none;
        opacity: 0.7;
        -webkit-transition: .2s;
        transition: opacity .2s;
    }

    .slider::-webkit-slider-thumb {
        -webkit-appearance: none;
        appearance: none;
        width: 10px;
        height: 10px;
        border-radius: 50%;
        background: white;
        border: 2px solid #22232B;
        cursor: pointer;
    }

    .slider::-moz-range-thumb {
        width: 10px;
        height: 10px;
        background: white;
        border: 2px solid #22232B;
        border-radius: 50%;
        cursor: pointer;
    }

    

    .minRange{
        position: relative;
        float: left;
        font-size: 0.7em;
    }

    .maxRange{
        position: relative;
        float: right;
        font-size: 0.7em;
    }

    .search-button{
        background: linear-gradient(to right, #33176C, #6B1D57);
        color:white;
        border-radius: 3px;
        padding: 10px;
        width: 100%;
        font-size: 0.7em;
        text-align: center;
        border: none;
    }

    .search-button img{
        position: relative;
        float: left;
    }
    
</style>
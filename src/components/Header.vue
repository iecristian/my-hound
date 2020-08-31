<template>
    <div class="header">
        <img class="logo" src="../assets/header-logo.png" alt="">
        <div class="header-menu">
            <button class="login">
                <img src="../assets/user.svg" alt="">
                <span>
                    SIGN IN
                </span>
                </button>
            <ul>
                <li>DOGS</li>
                <li>FAQS</li>
                <li>CONTACT US</li>
            </ul>
            
        </div>
        <div class="header-filters">
            <div class="search">
                <img src="../assets/search.png" alt="">
                <input type="text" class="filter-input" placeholder="Search">
                <select class="filter-select half-width" name="" id="">
                    <option value="time">By Breed</option>
                </select>

            </div>

        </div>
    </div>
</template>

<script>
export default {
    name: 'AppHeader',
    props:{
        
    }
}
</script>

<style scoped>
    .header{
        width: 100%;
        height: 250px;
        background-color: #FFFFFF;
        padding: 18px 120px 18px 120px;
    }

    .logo{
        width: 150px;
        position: relative;
        float:left;
    }

    .header-menu{
        width: 1170px;
    }

    ul{
        position: relative;
        float:right;
    }

    li{
        list-style: none;
        position: relative;
        float:left;
        margin: 10px;
        font-size: 1em;
        color: #22232B;
    }

    li:hover{
        color: #6B1D57;
        border-bottom: 2px solid #6B1D57;
    }

    .login{
        background-color: #FFFFFF;
        border: 1px solid #6B1D57;
        color: #6B1D57;
        border-radius: 5px;
        height: 55px;
        position: relative;
        float: right
    }

    
    .header-filters{
        width: 1170px;
        height: 103px;
        overflow: hidden;
    }

    .search{
        width: 1170px;
        height: 40px;
        overflow: hidden;
    }

    .filter-select, .filter-input{
        width: 60%;
        height: 30px;
        text-align: left;
        border:none;
        border-bottom: 1px solid #EBEBEB;
        margin: 10px;
        font-size: 0.8em;
        color: #22232B;
    }

    .half-width{
        width: 10%;
        margin-left: 5px;
        margin-right: 5px;
    }

    .filter-input::placeholder{
        margin-left: 10px;
        color:#22232B;
    }

    .filter-input:focus{
        outline:none;
         border-bottom: 1px solid #22232B;
    }

    .header-filters img{
        width:25px;
        margin-right: 20px;
        
    }

    @media screen and (max-width: 600px) {

        .login span{
            display: none;
        }

        .header{
            padding: 0;
        }

        .logo{
            margin-left: 120px;
            margin-top: 18px;
        }

        .header-menu ul{
            display: none;
        }

        .login{
            position: relative;
            float: left;
            padding: 5px;
            margin: 18px;
            width: 55px;
            height: 55px;
        }

        .login img{
            margin: 0;
            padding: 0;
        }

        .header-filters{
            width: 100%;
            position: relative;
            float: left;
        }

        .search{
            width: 100%;
        }

        .filter-select, .filter-input{
            width: 40%;
            margin-right: 0;
            margin-left:5px;
        }

        


        /*input*/

    }

    

</style>
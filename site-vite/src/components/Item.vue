<template>
    <div class="card">
        <a 
        :href="item.href">
            <img :src="item.img" alt="icon service" />
            <h3>{{ item.title }}</h3>
            <span>{{ item.description }}</span>
        </a>


    </div>
</template>
<script>
export default {
    props: ['item']
}
</script>

<style scoped>
div {
    display: block;
    width: 100px;
    margin: 30px 50px 30px 50px;
}

img {
 
    width: 100px;
    border-radius: 100px;
    

}
a {
text-decoration: none;
margin-left: 9px;
margin-top: 8px;
color: black;

}

a:hover {
    color: rgb(146, 19, 153);
}
h3 {
    font-weight: 900;
    font-size: 17px;
}

span {
    display: flex;
    flex-direction: column;
    font-size: 16px;
}
.card{
    background-color: rgba( 255, 255, 255, .5);
    display: flex ;
    justify-content: center;
    flex-direction: column;
    min-width: 120px;
    min-height: 150px;
    border: 1px solid grey;
    border-radius: 10%;
    opacity: .9;
    box-shadow: 0 0 2em grey;
    transition: box-shadow .5s;
    
}
.card:hover{
    opacity: 1;
    box-shadow: 0 0 4em grey;
}
@media ( max-width: 600px ) {
    div{
        margin: 20px 20px 20px 20px;
    }
    img{
        width: 70px;
        margin-left: 8px;
    }
    .card {
        min-width: 100px;
    min-height: 100px;
    }
    h3 {
        font-weight: 600;
    font-size: 13px;

    }
    span {

    font-size: 12px;
}
}
</style>
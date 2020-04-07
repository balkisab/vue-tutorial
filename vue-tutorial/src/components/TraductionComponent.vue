<template>
  <h1>Service de traductions médicales{{cmessage}}</h1>


</template>

<script>
export default {
  data (){
    return {
      message:[]
      }
  },
   name: 'TraductionComponent',
  props: {
    
    msg1: String,
     ip: String
  },
  ready: function () {

  }

}
</script>

<style >
 * {
	margin: 0px; 
	padding: 0px; 
	box-sizing: border-box;
}
body, html {
    width: 100%;
    /* min-height: 100vh; */
     display: -webkit-box;
    display: -webkit-flex;
    display: -moz-box;
    display: -ms-flexbox;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
    padding: 15px;
background-image: url(../assets/bg_3.jpg); 
}
.traduction{
   width: 960px;
    background: #fff;
    border-radius: 10px;
    overflow: hidden;
    padding: 15%;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;}
h1{
    font-family: Poppins-Bold;
    font-size: 27px;
    text-decoration: underline;
    color: #48C2C5;
    line-height: 1.2;
    text-align: center;
    margin-bottom:10%;
    padding-bottom: 54px;
    line-height: 1.5;
    margin-top:-20% ;
    height: 50px;
    border-radius: 25px;
    padding: 0 30px 0 68px;
}
img{
    width: 10%;
    margin-top: -10%;
    margin-left:45%
}
 .main-form{
    margin-left: 40%;
    padding-top:8%;
  }
select{ font-family: Poppins-Medium;
  font-size: 15px;
  line-height: 1.5;
  color: #48C2C5;
  display: block;
  /* margin-left: 50%; */
  width: 100%;
 padding-left: 3px;
  background: white;
  /* height: 50px; */
  border-radius: 25px;
  padding: -1 30px 0 68px;
  margin-bottom: 2%;
  margin-top: 2%;
  
}
.btn{
      margin-top:20%;
	font:Bold 13px Arial;
	background:#48C2C5;
	color:#fff;
	width:90px;
	border-radius:2px;
  border:none;
  margin-left:85%
  }
  .confirmer{

    margin-left:0
  }
  a {
    text-decoration: none;
    display: inline-block;
    padding: 8px 16px;
    margin-top:20%
  }
  
  a:hover {
    background-color: #48C2C5;
    color: black;
  }
  
  .previous {
    background-color: #f1f1f1;
    color: black;
  }
  
  .next {
    background-color: #f1f1f1;
    color: black;
  }
  .table{
    margin-top:20%;
}
tr th{
font-family: Poppins-Bold;
  font-size: 14px;
  color: #48C2C5;
  /* line-height: 1.2; */
  text-align: center;
}
td{
    font-family: Poppins-Medium;
    font-size: 15px;
    line-height: 1.5;
    color: #666666;
}  
  td input{
  font-family: Poppins-Medium;
  font-size: 15px;
  line-height: 1.5;
  color: #666666;
  display: block;
  width: 100%;
  background: white;
  /* height: 50px; */
  border-radius: 25px;
  padding: 0 30px 0 68px;
 }
 @media only screen and (max-width:768px) {
  .main-form{
    margin-left: 20%;
    padding-top:8%;
  }
  img{
    width: 20%;
    padding-top: 5%;
  }
 
 }
 @media only screen and (max-width:768px) {
 td input{
  font-family: Poppins-Medium;
  font-size: 14px;
  line-height: 1.5;
  color: #666666;
  display: block;
  width: 100%;
  background: white;
  /* height: 50px; */
  border-radius: 25px;
  padding-left:3px;
 }
}
</style>

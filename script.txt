

var curseur =document.querySelectorAll('#scales');
var p11=parseInt(document.getElementById('prix1').innerHTML,10);
var p22=parseInt(document.getElementById('prix2').innerHTML,10);
var p0=parseInt(document.getElementById('prix').innerHTML,10);
   
function increaseValue() {
    var value = parseInt(document.getElementById('number').value, 10);
    value = isNaN(value) ? 0 : value;
    value++;
    document.getElementById('number').value = value;
    

    document.getElementById('be1').addEventListener('click',cale1());
    function cale1(){
      //var p11=parseInt(document.getElementById('prix1').innerHTML,10);
      //var p22=parseInt(document.getElementById('prix2').innerHTML,10);
      //var p0=parseInt(document.getElementById('prix').innerHTML,10);
      var val=parseInt(document.getElementById('number').value,10);
      var pr1=120*val;

      document.getElementById('pe').innerHTML=`${pr1} $`;
      
      
      var val1=parseInt(document.getElementById('number1').value,10);
     var val2=parseInt(document.getElementById('number2').value,10);
     
      var tot=val1*p11+pr1+val2*p22;
    document.getElementById('output').innerHTML=` Shopping bag total: ${tot} $`;
    
    } 
   
  }
  
  function decreaseValue() {
    var value = parseInt(document.getElementById('number').value, 10);
    value = isNaN(value) ? 0 : value;
    value < 1 ? value = 1 : '';
    value--;
    document.getElementById('number').value = value;
   
    var val=parseInt(document.getElementById('number').value,10);
   
var val1=parseInt(document.getElementById('number1').value,10);
var val2=parseInt(document.getElementById('number2').value,10);

    document.getElementById('be2').addEventListener('click',cale());
    function cale(){
      var pr1=120*val;

      document.getElementById('pe').innerHTML=`${pr1} $`;
      var tot=val1*p11+pr1+val2*p22;
    document.getElementById('output').innerHTML=` Shopping bag total: ${tot} $`;
  
    } 
  }
  function increaseValue1() {
    
    var value = parseInt(document.getElementById('number1').value, 10);
    value = isNaN(value) ? 0 : value;
    value++;
    document.getElementById('number1').value = value;
    var val1=parseInt(document.getElementById('number1').value,10);
  
   
  var val=parseInt(document.getElementById('number').value,10);
  var val2=parseInt(document.getElementById('number2').value,10);
  var val1=parseInt(document.getElementById('number1').value,10);

document.getElementById('bm1').addEventListener('click',calm1());
    function calm1(){
      var pr2=500*val1;

      document.getElementById('pm').innerHTML=`${pr2} $`;
      var tot2=val*p0+pr2+val2*p22;
     // alert(document.getElementById('output').innerHTML);
    document.getElementById('output').innerHTML=` Shopping bag total: ${tot2} $`;
  
    } 
  }
  
  function decreaseValue1() {
    var value = parseInt(document.getElementById('number1').value, 10);
    value = isNaN(value) ? 0 : value;
    value < 1 ? value = 1 : '';
    value--;
    document.getElementById('number1').value = value;
    var val1=parseInt(document.getElementById('number1').value,10);
    var val=parseInt(document.getElementById('number').value,10);
  var val2=parseInt(document.getElementById('number2').value,10);


    document.getElementById('bm2').addEventListener('click',calm2());
    function calm2(){
      var pr1=500*val1;

      document.getElementById('pm').innerHTML=`${pr1} $`;
      
      var tot2=val*p0+pr1+val2*p22;
      // alert(document.getElementById('output').innerHTML);
     document.getElementById('output').innerHTML=` Shopping bag total: ${tot2} $`;
    } 
    
    
  }
 
  

  function increaseValue2() {
    var value = parseInt(document.getElementById('number2').value, 10);
    value = isNaN(value) ? 0 : value;
    value++;
    document.getElementById('number2').value = value;
    var val2=parseInt(document.getElementById('number2').value,10);
    var val=parseInt(document.getElementById('number').value,10);
   var val1=parseInt(document.getElementById('number1').value,10);
  
    
    var bs=document.getElementById('bs1');
 
    bs.addEventListener('click',cal1());
  function cal1(){
             var pr2=80*val2;
             //console.log(pr2);
              document.getElementById('ps').innerHTML=`${pr2} $`;
              var tot2=val*p0+pr2+val1*p11;
              // alert(document.getElementById('output').innerHTML);
             document.getElementById('output').innerHTML=` Shopping bag total: ${tot2} $`;
          
            }  
    
  }
 
 
  
  function decreaseValue2() {
    var value = parseInt(document.getElementById('number2').value, 10);
    value = isNaN(value) ? 0 : value;
    value < 1 ? value = 1 : '';
    value--;
    document.getElementById('number2').value = value;
    var val2=parseInt(document.getElementById('number2').value,10);
   // var val2=parseInt(document.getElementById('number2').value,10);
    var val=parseInt(document.getElementById('number').value,10);
   var val1=parseInt(document.getElementById('number1').value,10);
    document.getElementById('bs2').addEventListener('click',cal2());
    function cal2(){
      var pr1=80*val2;

      document.getElementById('ps').innerHTML=`${pr1} $`;
      var tot2=val*p0+pr1+val1*p11;
              // alert(document.getElementById('output').innerHTML);
             document.getElementById('output').innerHTML=` Shopping bag total: ${tot2} $`;
          
  
    } 
    
    
  }


 
  //var arr=Array.from(document.quarySelectorAll('#scales'));
  
  //var message= document.getElementById('output');
  //var px=document.querySelectorAll('#prix');
 

function total(){
  



    for (let i in curseur){
     //alert(document.getElementById('prix'));
     //alert(curseur[i].checked);
           
        if (curseur[i].checked===true){
       //var bouton=document.getElementsByClassName('value-button');
   
            var tot=val1*p1+val*p+val2*p2;
            document.getElementById('output').innerHTML=` Shopping bag total: ${tot} $`;

        }
    }
}



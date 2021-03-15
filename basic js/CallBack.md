## . Callback 

là cách đảm bảo code sẽ không hoạt động trước khi các code khác hoàn thành việc thực thi.

````javascript
function first(callback){
    // Simulate a code delay
    setTimeout( function(){
      console.log(1);
      callback();
    }, 500 );
  }
  function second(){
    console.log(2);
  }
  first(second)
````
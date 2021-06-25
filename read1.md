## Node Ecosystem, TDD, CI/CD
#### Array.map()
*map() Manipulate the data from the array and set them into a new Array with the same length of orginal array also without changing the data in the original array that we send. the map calls a provided callback function once for each element in an array, in order, and constructs a new array from the results. a callback is invoked only for indexes of the array which have assigned values*

#### Array.reduce()
*array is looping in array element and make some specific operation then return the result.*

#### superagent()
function getResultFromApi(req,res){

const url='http://hp-api.herokuapp.com/api/characters';

superagent.get(url).then(result=>{

return result.body.map(obj=>

new Hp(obj));

}).then(result=>{ res.render('index',{sendRes:result})

});

}


#### async await function
Executed first ==>show first Even if there is another promise not Executed yet , Depends on
which finsh his Executed first
which have the request that reaches first
you can worksomething else no need to wait the response , so try to do but not now
your code continue work without stop

#### Are all callback functions considered to be Asynchronous ??
No, we can use callback as synchronous or Asynchronous, it depends on sitution that we are in
# npm-jlinq

jlinq.from(data.source)
  .starts('first', 'a')
  .select();
 
//complex queries - no need to repeat names
//when querying the same field
jlinq.from(data.source)
    .starts('first', 'a')
    .or('b')
    .or('c')
    .sort('last')
    .select();
 
//sorting - multiple field
jlinq.from(data.source)
  .greater('age', 40)
  .sort('age', 'name');
  .select();

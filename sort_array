// sort an array
/*function change(a,b)
 {
  var c;
   c = a;
   a = b;
   b = c;
console.log( "values  a" + " " + a + " " + "b : " + " " + b);
 }*/
//var tab=[3,2];
//change(tab[0],tab[1]);
//tab[0]=tab[1];
//tab;
function trier()
{
  var tab = [3,2,1,7,5];                 
  var size = tab.length;              
  for( var i = 0 ;i < size; i++)                                           
      {
       for(var j = 0; j < size; j++)
          {
           if(tab[i] < tab[j])  // <  croissant,    > decroissant
             {
               let int = tab[j];
               tab[j] = tab[i];
                tab[i] = int;
               console.log("mouve :" + " " +tab + "\n");
             }
           }
         }
console.log( "values :" +tab); 
}
trier();

// reorganiser un tableau de sous tableaux en un tableau

const flatten = (tab) => {
  if (tab === null || tab.length === 0) return [];
  const newTab = [];
  flattenHelper(newTab, tab);
  return newTab;
};

const flattenHelper = (newTab, currentTab) => {
  for (let i = 0; i < currentTab.length; i++) {
    if (Array.isArray(currentTab[i])) {
      flattenHelper(newTab, currentTab[i]);
    } else if (currentTab[i] !== null) {
      newTab.push(currentTab[i]);
    }
  }
};

const arr = [1, [[2], 3, 4, null], [[5]],[6,7]];
console.log(flatten(arr)); // 1,2,3,4,5,6,7

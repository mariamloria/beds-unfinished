let attachmentprice = Number(document.getElementById("attachmentprice").innerText);
let price = Number(document.getElementById("price").innerText);
let maxprice = price+(2*attachmentprice);
document.getElementById("plus").addEventListener(
  "click", ()=>{ 
    if(price >= maxprice){
      price == maxprice;
      document.getElementById("price").innerText = maxprice; 
    }else{
      price+=attachmentprice;
    document.getElementById("price").innerText = price;
    }
  }
)
let minprice = Number(document.getElementById("price").innerHTML);

document.getElementById("minus").addEventListener(
  "click", ()=>{ 
    if(price <= minprice){
      price == minprice;
      document.getElementById("price").innerHTML = minprice; 
    }else{
      price-=attachmentprice;
      document.getElementById("price").innerText = price;
    }
  }
)

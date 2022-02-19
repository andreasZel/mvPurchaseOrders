# Process that was followed

1) Files :

    --(ListOfPurchases.html)
    First i created the .html file that will show the JSON data. An hidden
    div is also included for the pop up.

    --(ListStyle.css)
    Then a .css file was created to make the code more compact and the html
    more visible to the reader.

    --(Get_Edit_JSON.js)
    Finaly, the .js file contains the JSON data as local variable (DataList) as 
    well as 4 functions.
        -- displayList() :
        Is called on window.onload and creates li elements in the ul of the html file
        that contains the asked format { PurchaseOrderTypeAbbreviation } – { PurchaseOrderNo }.
        The id of each li element is the PurchaseOrderId because an event listener is also added 
        to each element to open the popup menu that calls showMoreInfo(P_id) function.

        -- enablePopUp() :
        Shows the pop up

        -- closepopup()  :
        Closes the popup and the content of the table.

        -- showMoreInfo(P_id) :
        Pass through the mvPurchaseOrders, if the id that called the function is the id of the current 
        object we pass by, first show PurchaseOrderAddress, PurchaseOrderContactPerson, PurchaseOrderStatus and then create row elements in the table of html that contains the PurchaseOrderDetails. 

2) CV similar projects

   The chat app that i created with a co-student used some of the elements that was needed here, mainly the pop ups and visulisation (CSS, HTML) and the dynamic creation of elements (js) but 
   i never used or processed JSON data. The main data we processed were in application/x-www-form-urlencoded format in AJAX calls.  
      

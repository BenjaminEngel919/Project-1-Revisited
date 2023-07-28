# Project-1-Revisited


![image](https://github.com/BenjaminEngel919/Project-1-Revisited/assets/126991382/f299eaa5-f831-48bc-b683-7cc022e98139)



Based on the above plot, the most impactful features are 'Outlet_Size', 'Outlet_Identifier_OUT049', and 'Outlet_Identifier_Out35'.

What this means is that for every 1 point increase in 'Outlet_Size', the predicted sales price increases by 2.330360e+14.

For every 1 point increase in 'Outlet_Identifier_OUT049', the sales price decreases by -1.690113e+14.

Finally, for every 1 point increase in 'Outlet_Identifier_OUT035', the predicted sales price increases by 1.152946e+14.


![image](https://github.com/BenjaminEngel919/Project-1-Revisited/assets/126991382/60d21efd-3bac-4d64-8420-857c26857184)



The above plot depicts the top 5 most important features in predicting price in our random forest model with the 'Item_MRP' feature being the obvious most important.

![image](https://github.com/BenjaminEngel919/Project-1-Revisited/assets/126991382/ab6bf6ad-3dcd-4cec-876a-1223015b05e3)

HAP summary plot vs top 5 most important features

![image](https://github.com/BenjaminEngel919/Project-1-Revisited/assets/126991382/ef9c5df0-04be-4aa6-a0a4-20f9f8c726a6)


Are they the same features in both? If not, what's different?

Top two values are the same in each plot. The remaining top 5 are in the top 7 of the SHAP plot. Just a slightly different order.


![image](https://github.com/BenjaminEngel919/Project-1-Revisited/assets/126991382/0e595560-fd5b-4507-9100-2751b6a6eabc)


Top 3: Item_MRP, Outlet_type_Grocery Store and Outlet_Identifier_OUT027.

Item_MRP influences the model mostly positively. The red is on the right (positive), higher values of this feature increase the chance the prediction will be fail.

Outlet_type_Grocery Store influences the model mostly negatively. If the red is on the left (negative), higher values of this feature decrease the chances the prediction will be fail.

Outlet_Identifier_OUT027 influences the modle mostly positively. The red is on the right (positive), higher values of this feature increase the chance the prediction will be fail.


Lime

![image](https://github.com/BenjaminEngel919/Project-1-Revisited/assets/126991382/3bed2e35-000b-4460-a5c6-46ce9d5b8d61)

![image](https://github.com/BenjaminEngel919/Project-1-Revisited/assets/126991382/931a7b3b-ae7b-455d-9f37-1240981b8297)


The two lime results above show the importance of each feature in predicting the sales for the store netting a high sales value of 13086 and the store netting a low sales value of 50 as selected previously. For both stores, the features that are influencing their respective sales the most are the 'Outlet_Type_Grocery_Store' and 'Item_MRP'. Between the two stores, the store with the higher sales has a higher 'Item_MRP' than the store with lower sales. This may suggest that the store with higher sales may mark up their product more or may have more of a product offering/variation that the other store. The 'Outlet_Type_Grocery_Store' may describe a different type of store that may be more or less be convenient to customers that may further describe the variation in sales between the two stores.

Force Plot

![image](https://github.com/BenjaminEngel919/Project-1-Revisited/assets/126991382/64e142ac-cce2-48c1-a08b-36b91efbdb17)


![image](https://github.com/BenjaminEngel919/Project-1-Revisited/assets/126991382/e81b374f-11b2-4207-96a3-7dba930cce4c)


According to both force plots above, the feature that most influenced the predictions for the stores with high and low sales was the Outlet_Establishment_Year. The higher producing store was from 1999 and the lower producing store was from 1998.

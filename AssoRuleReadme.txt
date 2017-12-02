The Dataset is: mushroom.dat
The Notebook is: Assignmen2ItemSetAndAssociationRules.ipynb

The dataSet is from machine learning database. I got the data from the site Manning in Action site. 
I bought the book: Machine Learning in Action (Peter Harrington).  I downloaded the source code and related dataSet.

The dataset contains 8124 observations and 23 attributes (see below) . Each attributes is a nominal type.
Example of the original data.
p,x,s,n,t,p,f,c,n,k,e,e,s,s,w,w,p,w,o,p,k,s,u
e,x,s,y,t,a,f,c,b,k,e,c,s,s,w,w,p,w,o,p,n,n,g

According to the author of the book the data is translated to this:
2 6 9 13 24 28 35 36 39 51 52 58 59 63 73 83 85 88 90 93 104 112 119 
2 4 9 13 24 28 35 36 39 51 52 58 59 63 73 83 85 87 90 93 105 112 119 

An I used the translated dataSet for the assignment (ItemSet and Association Rule algorithm)

To mini minimize the number of ItemSet after testing many support  level I used the support level equals to 90%.

To have some rule I fixed the confidence level equal to 60%.

The Result is:

['34', '86'] => ['85'] (support: 0.97 confidence: 1.00)
['34'] => ['85'] (support: 0.97 confidence: 1.00)
['86'] => ['85'] (support: 0.98 confidence: 1.00)
['90'] => ['85'] (support: 0.92 confidence: 1.00)
['34'] => ['86'] (support: 0.97 confidence: 1.00)
['34', '85'] => ['86'] (support: 0.97 confidence: 1.00)
['86'] => ['34'] (support: 0.97 confidence: 1.00)
['86', '85'] => ['34'] (support: 0.97 confidence: 1.00)
['85'] => ['86'] (support: 0.97 confidence: 0.98)
['85'] => ['34'] (support: 0.97 confidence: 0.97)
['85'] => ['90'] (support: 0.97 confidence: 0.92)


Interpretation of some rules:

'34', '86'] => ['85'] (support: 0.97 confidence: 1.00) 
means 97% of the dataSet (transactions contains the item 34, 86 and 85) and each transaction that contains 34 and 86 
contains also 85 with certitude (100%)

['90'] => ['85'] (support: 0.92 confidence: 1.00)
 means 92% of the dataSet (transactions contains the item 90 and 85) 
and each transaction that contains 90 contains also 85 with certitude (100%)

['85'] => ['86'] (support: 0.97 confidence: 0.98) 
means 97% of the dataSet (transactions contains the item 85 and 86) 
and each transaction that contains 85 contains also 85 with a probability of 98%

Structures of the DataSet:

Attribute Information:

0: classes: edible=e, poisonous=p
1. cap-shape: bell=b,conical=c,convex=x,flat=f, knobbed=k,sunken=s 
2. cap-surface: fibrous=f,grooves=g,scaly=y,smooth=s 
3. cap-color: brown=n,buff=b,cinnamon=c,gray=g,green=r, pink=p,purple=u,red=e,white=w,yellow=y 
4. bruises?: bruises=t,no=f 
5. odor: almond=a,anise=l,creosote=c,fishy=y,foul=f, musty=m,none=n,pungent=p,spicy=s 
6. gill-attachment: attached=a,descending=d,free=f,notched=n 
7. gill-spacing: close=c,crowded=w,distant=d 
8. gill-size: broad=b,narrow=n 
9. gill-color: black=k,brown=n,buff=b,chocolate=h,gray=g, green=r,orange=o,pink=p,purple=u,red=e, white=w,yellow=y 
10. stalk-shape: enlarging=e,tapering=t 
11. stalk-root: bulbous=b,club=c,cup=u,equal=e, rhizomorphs=z,rooted=r,missing=? 
12. stalk-surface-above-ring: fibrous=f,scaly=y,silky=k,smooth=s 
13. stalk-surface-below-ring: fibrous=f,scaly=y,silky=k,smooth=s 
14. stalk-color-above-ring: brown=n,buff=b,cinnamon=c,gray=g,orange=o, pink=p,red=e,white=w,yellow=y 
15. stalk-color-below-ring: brown=n,buff=b,cinnamon=c,gray=g,orange=o, pink=p,red=e,white=w,yellow=y 
16. veil-type: partial=p,universal=u 
17. veil-color: brown=n,orange=o,white=w,yellow=y 
18. ring-number: none=n,one=o,two=t 
19. ring-type: cobwebby=c,evanescent=e,flaring=f,large=l, none=n,pendant=p,sheathing=s,zone=z 
20. spore-print-color: black=k,brown=n,buff=b,chocolate=h,green=r, orange=o,purple=u,white=w,yellow=y 
21. population: abundant=a,clustered=c,numerous=n, scattered=s,several=v,solitary=y 
22. habitat: grasses=g,leaves=l,meadows=m,paths=p, urban=u,waste=w,woods=d

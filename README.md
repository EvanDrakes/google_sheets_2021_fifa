# Cleaning Project

## Making Heights the same Value

### Turning centimeters into inches
```
=SUBSTITUTE(M2,"cm"," ",1)
=CONVERT(N2,"cm","in")
=ROUND(O2, 1)
```
### Turning feet'inches" into inches
```
=SUBSTITUTE(M863,"'","", 1)
=SUBSTITUTE(N863, """","", 1)
=MULTIPLY(LEFT(O863, 1), 12)
=CONCATENATE(ADD(RIGHT(O863, 1),P863),"in") 
```
## Seperating Month, Day, Year
```
=TEXT(V2,"mmm")
=TEXT(V2,"dd")
=TEXT(V2,"yyyy")
```
## Turning Columns into Integer Columns
```
=if((right(AA2,1))="K",(value(left(AA2,(len(AA2))-1)))1000,if((right(AA2,1))="M",(value(left(AA2,(len(AA2))-1)))1000000,""))
```
[Final Results](https://docs.google.com/spreadsheets/d/16fTAHn8iMF_Fcwv8Ix4Yo0neNEC92R_i46uMAAhecFg/edit#gid=1084324460)

## 1NF: A cell should contain just atomic values.
## 2NF: (must be independent of Partial dependency): Any non prime attrib should be dependent on entire candidate key,
   not on a part of candidate key. P => N

   Essential Attrib: The attrib that do not have any incoming edges.
   Find candidate key, the attribs that can define all the attrib in a relation
   All attribs in a candidate  key are prime attributes // non-prime attrib
   
   Primary key value should not be null, but one can be null right?
   AB->CD
    -   -> 
    -----
    
    B leader, so make it leader with another table.
    R1 ( A B D )
    R1 ( B C )
    
## 3NF: ( must be independent of transitive dependency ): When non prime is dependent on non prime attrib  NP => NP 

    R( A-B=>C->D )  from AB we can find C and from C we can find B. So AB are candidate key, A, B are prime attrib
    R1( A-B => C)
    R2( C => D )
   
## BCNF: P/NP => P  if A => B    then A should be a Super key
   
   R ( A-B=><-C) from AB find C and from C again find B
   

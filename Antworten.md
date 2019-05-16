1:

  a) (((250 * 1024) * 1024) * 1024) / 1024 = 262 144 000‬ Blöcke
  
  b) Gleiche Anzahl wie Blöcke
  
  c) Wir müssen bei jedem Entry die BlockId und die nächste Adresse angeben also: log_2(anzBlöcke) = 27.966 also verwenden wir 32 bit
  
  d) AnzBlöcke * sizeEntry = 8388608000 bit / 8 / 1024 / 1024 = 1000MB
 
2: Suche in Block: 107834590 / 1024 = 105307.2168 -> 105308

  a) wenn anzBlöcke < 10 -> directBlock n
  
     -||-          < 256 + 10 = 266 -> singleIndirect
     
     -||-          < 256² + 266 = 65802 -> doubleIndirect
     
     -||-          < 256³ + 65802 = 16843018 -> tripleIndirect
     
     256² + 155*256 + 92 = 105308
     
   b) wir lesen die data aus dem block nachdem wir 105308 Blöcke weitergesprungen sind

3: 

4: 

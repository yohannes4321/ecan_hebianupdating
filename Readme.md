second truth value mean 0.05 confidence =0.1

defualt_k =800

cval=0.2

convert confidence to counts

for the first truth value 

count1=defualt_k * confidence/(1-confidence)
count1 =800 * 0.9 /(1-0.9) = 720/0.1 =7200

for the second truth value 

count2 =defualt_k*confidence /(1-confidence)=800*0.1/(1-0.1)=80/0.9=88.89


step2 Compute the new count 

count_new=count1+count2 -min(count1,count2)*CVAL

count_new = 7200 + 88.89 -(88.89*0.2)

count_new =7200 + 88.89 -17.78 =7271.11



step3 compute the new mean

mean_new= mean*count1 + mean *count 2 /(count1+count2)

mean_new =0.01 *7200 + 0.05 * 88.89/(7200 + 88.89)
mean_new = 72 + 4.4445/(7288.89)=76.4445/7288.89 = 0.01049

step4 compute the new confidence 

cofidence_new= count _new /count_new + Defualt_k
confidence_new = 7271.11/7271.11 +800
confidence_new=7271.11 /8071.11=0.901

the merged truth value is mean 0.01049
confidence=0.901
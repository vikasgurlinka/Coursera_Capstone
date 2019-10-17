# Coursera_Capstone


https://towardsdatascience.com/exploring-chandigarh-india-using-foursquare-and-zomato-api-1d4501291320

https://github.com/ParthPathak27/Applied-Data-Science-Capstone-Project

https://github.com/chriswjamo/Coursera_Capstone/blob/master/Capstone%20Final%20Project%20-%20Final%20Version_Git.ipynb

https://github.com/pezLyfe/IBM-Capstone



for i in range(0,len(df['categories'])):
	try:
		cat.append(df['categories'][i][0]['name'])
	except:
		cat.append(None)


for i in range(0,len(df['categories'])):
	if cat[i]==None : cat[i]=name[i]


for i in range(0,len(df['categories'])):
	print("{} --> {}".format(name[i],cat[i]))

for i in range(0,len(df['categories'])):
	if re.search('Restaurant',cat[i]):print("{} --> {}".format(name[i],cat[i]))


df_fil=df_fil.drop(['location.labeledLatLngs', 'location.cc'], axis=1)
df_fil.head(2)
cols=['id','name', 'categories','location.lat','location.lng' ,'location.crossStreet', 
      'location.address','location.distance', 'location.postalCode','location.formattedAddress','location.city', 'location.state',
      'location.country']
df_fil = df_fil[cols] 
df_fil.head(2)

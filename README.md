# ics31assignment2parth
#(h) restaurants
from collections import namedtuple
Restaurant = namedtuple('Restaurant', 'name cuisine phone dish price')
# Restaurant attributes: name, kind of food served, phone number, best dish, price of that dish
RC = [
    Restaurant("Thai Dishes", "Thai", "334-4433", "Mee Krob", 12.50),
    Restaurant("Nobu", "Japanese", "335-4433", "Natto Temaki", 5.50),
    Restaurant("Nonna", "Italian", "355-4433", "Stracotto", 25.50),
    Restaurant("Jitlada", "Thai", "324-4433", "Paht Woon Sen", 15.50),
    Restaurant("Nola", "New Orleans", "336-4433", "Jambalaya", 5.50),
    Restaurant("Noma", "Modern Danish", "337-4433", "Birch Sap", 35.50),
    Restaurant("Addis Ababa", "Ethiopian", "337-4453", "Yesiga Tibs", 10.50) ]
print(RC[2].name)
print(RC[0].cuisine == RC[-1].cuisine)
print(RC[-1].dish)
RC.sort() #(h.5)
for l in range(0,len(RC)): # might be a better way to do this
    print(RC[l].name) # tried printing 'print(RC[].name' w/o for loop but didn't work
print(RC[-1].dish) #(h.6)

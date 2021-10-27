A.   What architecture will you recommend for the solution and why?
Ans: We will follow Mulesoft API architecture.
	 1. Because it donot exposed the backend data and codes and only exposes the importand things to the customers.
	 2. Process APIs are less volatile compared to System APIs.
	    If we use normal API architecture, if some lower level architectute chnages, we need to change the whole API structure.
		Therefore Mulesoft architectute will be preffered.
		
B.   How would you design the solution?
Ans: Using API led connectivity appoach of mulesoft..
     1. We need to create a REST API for INDIGO flight booking [SYSTEM]
	 2. We need to create a SOAP API for TAAJ Hotel booking [SYSTEM]
	 3. CSV file for Car Booking [SYSTEM]
	 4. Book My Holiday will use both the rest and soap apis along with this csv file for respective bookings [PROCESS]
	 
C.   What non-functional requirements are important while designing the solution ?
Ans: x-Token [Client_id and Client_secret]
	 HTTP Caching
     
D.   How future proof is your solution when it comes to onboarding to new partners/destinations
Ans: If new partners comes for Car Booking, we dont need to change anything in API.
     If any new flight partner like SpiceJet come, we need to add a new system api and connect that to the process api.
	 Same for Hotel Booking.
	 
E.   What is your proposition for giving personalized offerings to the customers?
Ans: We will also expose a Offers section the the main App which will reflect mouth watering cashback offers.
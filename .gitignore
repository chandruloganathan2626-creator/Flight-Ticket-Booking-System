2# flight ticket booking system

#available flights
flights = {
    1:{"route": "chennai to banglore","price":2500},
    2:{"route":"chennai to madurai","price":2000},
    3:{"route":"chennai to mumbai","price":5000},
    4:{"route":"chennai to hyderabad","price":6500}
}

Tax_rate = 0.20

print("===== flight ticket booking system =====\n")

#display available flights
print("available flights:")
for flight_id, details in flights.items():
    print(f"{flight_id}.{details['route']}-{details['price']}")

#select flight
flight_choice = int(input("\nenter flight number:"))

if flight_choice in flights:
    selected_flight = flights[flight_choice]

    #number of passengers
    passengers = int(input("enter numberof pssengers:"))

    #cost calculation 
    base_cost = selected_flight["price"] * passengers
    tax = base_cost * Tax_rate
    total_cost = base_cost + tax

    print("\nbooking details")
    print("----------------")
    print("flight:",selected_flight["route"])
    print("passenger:",passengers)
    print("base fare:",base_cost)
    print("Tax (10%):",tax)
    print("total cost:",total_cost)

    #confirmation
    confirm = input("\nconfirm booking? (yes/no):").lower()
    
    if confirm == "yes":
        print("\n===== BOOKING CONFIRMED =====")
        print("Flight:", selected_flight["route"])
        print("Passengers:", passengers)
        print("Total Paid: ₹", total_cost)
        print("Status: Confirmed")
    else:
        print("\nBooking Cancelled.")
else:
    print("Invalid Flight Selection!")

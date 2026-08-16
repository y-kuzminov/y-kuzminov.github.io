# API Testing — Hillel Auto

End-to-end API test flow for a car management application.

### Covered scenario
1. Sign up (unique user every run)
2. Edit user profile (name + last name)
3. Change distance units to miles
4. Add a car
5. Update car mileage
6. Add fuel expense
7. Delete car
8. Delete user

### Technical details
- All requests have assertions (status code + response body)
- Pre-request scripts generate unique email and names
- Collection is designed to be run via Collection Runner / Newman
- Base URL: `https://qauto.forstudy.space/api`

### How to run
1. Import the collection into Postman
2. Set environment variable `Base_URL` if needed
3. Run the collection — a new user is created automatically each time

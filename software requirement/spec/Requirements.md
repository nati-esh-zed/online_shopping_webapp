# Requirements

## System

### Operational

- A web-application is preferred as it is platform independent and internet is unavoidable.
- A web-server must be selected and setup to handle at least 10,000 customers for starter.
- Web server capabilities should be scaled up to meet increasing demand.
- A frontend library should be used to generate a single page web-application and generate
  the view components dynamically by fetching the required information from the backend web-server.

### Legal

- The company must have legally registered and verified business document in the
  country/area where it operates.
- An End User License Agreement(EULA) must be properly written and provided for end users.
  Consider consulting lawyer.
- Lawyers must be hired for consulting and to handle cases requiring legal action.

## Users and User Accounts

- User account creation, session management and administration.
- There are customer, vendor, administrator, employees which include manager, lawyer and courier.

### Vendors

- Vendors must be able to register items in stock given the required information
  such as brand, name, price and quantity.
- Vendors must be able to view and modify items registered in their stock.
- Vendors must be able to search and filter using some criteria such as brand, price range and area
  from their own stock and other's stock to checkout the competition.

### Customers

- Customers must be able to search and filter using some criteria such as brand, price range and area
  from registered items and then must be able to select items and put them in a cart.
- Customers must be able to view and modify the items in their cart. Which are
  - View the items in a list
  - View the total price
  - Remove items from the list
  - Increase or decrease the quantity of items
- Customers must be able to pay through supported e-payment systems with ease.
- Customers must be able to view and keep track of, and cancel their orders.
  Status, notifications, location, delivery time should be considered.

### Employees

#### Administrator

- There must be one administrator account.
- Administrator must be able to:
  - View and manage employees.
  - Registration and removal of employees.
  - Setting the salaries of the employees.
  - Backing up data.

#### Managers

- Managers must be able to hire and manage couriers. Management includes:
  - Hiring and firing couriers.
  - Assigning delivery tasks to couriers.
  - Handling failing delivery cases and conflicts.
  - Consulting and assigning lawyers to cases that require legal action.

#### Lawyers

- Layers handle all legal issues for the company.

#### Couriers

- Couriers handle safe and fast delivery of items.
- Couriers must be able to:
  - View and accept or reject delivery tasks.
  - Contact their manager, the vendor and the customer through safe and secure means.
  - Complete delivery tasks.

## Payment

- Payment should be done though a common API and with available e-payment systems.
- Customers, vendors and employees should have a checking account that supports e-payment
  and it must be registered in the system.
- When customers pay for a purchase the money must be temporarily put in a common
  'customers-holding' checking account until successful or unsuccessful delivery of items
  from vendor to customer through a courier.
  - Upon successful delivery the money must be transferred to the corresponding vendors'
    registered checking account with deducted fees.
  - Upon unsuccessful delivery the money must be transferred back to the customer's registered
    checking account.
- Deducted fees include tax, service fees, delivery costs and transaction costs.

## Item Exchange

- Item exchange may occur from vendor to courier, courier to customer, courier to manager,
  manager to courier and courier to vendor.
- The must be a form provided for item exchange. That form must include:
  - List of items to be exchanged with important information such as quantity and expected condition.
  - A checkbox for each item to signify acceptance or rejection of the item.
    The checkbox must either be marked or crossed.
  - A reason-for-rejection form items presented.
    Such reasons include items presented in an unexpected condition (not as advertised or damaged).
  - A submit button or a signature box if it is paper form.
- No one should accept items presented in an unexpected condition as they will take responsibility.
- The person who has items in their possession takes responsibility for the safety of those items.
  And the company is responsible for providing and handling a trust worthy and reliable courier
  and handles all legal issues regarding safe item delivery and accidents or scams.

## Shubham's Approach

#### Weather Monitoring System:
- In the Weather Monitoring System, the Observer pattern is used to create a weather station that notifies multiple display devices (observers) about changes in weather conditions. The WeatherData class acts as the subject, maintaining a list of observers and providing methods to subscribe and unsubscribe observers. The DisplayDevice classes serve as concrete observers, implementing the update method to handle and display the received weather data. The WeatherStation class notifies all registered observers when new weather data is available.

#### Vehicle Manufacturing System:
- In the Vehicle Manufacturing System, the Factory Method pattern is utilized to create different types of vehicles based on user input. The abstract Vehicle class defines the interface for all vehicle objects, while the concrete vehicle subclasses (Car, Motorcycle, Truck) implement the Vehicle interface with specific attributes and details. The VehicleFactory abstract class declares the factory method create_vehicle(), and the concrete factory subclasses (CarFactory, MotorcycleFactory, TruckFactory) implement this method to create the corresponding vehicle objects based on user input. The code prompts the user to input a vehicle type, selects the appropriate factory based on the input, creates the desired vehicle object using the factory, and displays its attributes.



## Comparision:

#### Weather Monitoring System:

- In Shubham's code, the property decorator is used to define getter methods for the temperature, humidity, and pressure properties in the WeatherData class. The property decorator allows you to define methods that can be accessed like attributes, providing a more intuitive and convenient way to retrieve and manipulate data.
- By using the @property decorator, these methods are transformed into properties, allowing them to be accessed as attributes.
- For example, instead of calling weather_data.temperature() as a method, you can simply access it as weather_data.temperature. The property decorator makes it look like a direct attribute access, providing a more natural syntax.
- In Shubham's code, the properties temperature, humidity, and pressure provide read-only access to the private variables _temperature, _humidity, and _pressure. The getter methods simply return the values of these variables.

#### Vehicle Manufacturing System:

- We used almost similar approach except for specific vehicle properties, the hierarchy of the factory classes, and the user input handling. 

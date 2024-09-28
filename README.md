-import java.util.ArrayList;
import java.util.List;

public class Car {
    private int carId;
    private String brand;
    private String model;
    private int year;
    private double rentalPricePerDay;
    private boolean availability;

    public Car(int carId, String brand, String model, int year, double rentalPricePerDay) {
        this.carId = carId;
        this.brand = brand;
        this.model = model;
        this.year = year;
        this.rentalPricePerDay = rentalPricePerDay;
        this.availability = true;
    }

    public String getDetails() {
        return "Car ID: " + carId + ", Brand: " + brand + ", Model: " + model + ", Year: " + year;
    }

    public void setAvailability(boolean availability) {
        this.availability = availability;
    }

    public boolean isAvailable() {
        return availability;
    }
}

public class Customer {
    private int customerId;
    private String name;
    private String contactInfo;

    public Customer(int customerId, String name, String contactInfo) {
        this.customerId = customerId;
        this.name = name;
        this.contactInfo = contactInfo;
    }

    public void registerCustomer() {
        
    }

    public void updateInfo(String name, String contactInfo) {
        this.name = name;
        this.contactInfo = contactInfo;
    }
}

public class RentalAgency {
    private String agencyName;
    private String location;
    private List<Car> carsList;

    public RentalAgency(String agencyName, String location) {
        this.agencyName = agencyName;
        this.location = location;
        this.carsList = new ArrayList<>();
    }

    public void addCar(Car car) {
        carsList.add(car);
    }

    public void removeCar(Car car) {
        carsList.remove(car);
    }

    public List<Car> listAvailableCars() {
        List<Car> availableCars = new ArrayList<>();
        for (Car car : carsList) {
            if (car.isAvailable()) {
                availableCars.add(car);
            }
        }
        return availableCars;
    }
}

public class RentalTransaction {
    private int transactionId;
    private Car car;
    private Customer customer;
    private Date rentalDate;
    private Date returnDate;

    public RentalTransaction(int transactionId, Car car, Customer customer, Date rentalDate, Date returnDate) {
        this.transactionId = transactionId;
        this.car = car;
        this.customer = customer;
        this.rentalDate = rentalDate;
        this.returnDate = returnDate;
    }

    public void createRentalTransaction() {
  

    public double calculateRentalFee() {
      
        return 0.0;
    }
}


<!---
CaxtonMbiu696/CaxtonMbiu696 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

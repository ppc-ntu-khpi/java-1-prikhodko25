# Звіт
## Customer
### Код програмии

package domain;
public class Customer {
    private int ID = 1;
    private boolean isNew = true;
    private double total = 1000;
    public Customer() {
    }
    public Customer(int ID, boolean isNew, double total) {
        this.ID = ID;
        this.isNew = isNew;
        this.total = total;
    }
    public int getID() {
        return ID;
    }
    public void setID(int ID) {
        if (ID > 0) {
            this.ID = ID;
        }
    }
    public boolean isNew() {
        return isNew;
    }
    public void setStatus(boolean isNew) {
        this.isNew = isNew;
    }
    public double getTotal() {
        return total;
    }
    public void setTotal(double total) {
        if (total >= 0) {
            this.total = total;
        }
    }
    public void displayCustomerInfo() {
        System.out.println("Customer ID: " + ID);
        System.out.println("Is new customer: " + isNew);
        System.out.println("Total purchases are: " + total);
    }
}
### Результат
![alt-текст](https://github.com/ppc-ntu-khpi/java-1-prikhodko25/blob/main/src/domain/placeholder.png)

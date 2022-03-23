# -Write-a-program-to-create-a-class-Book-with-the-following--attributes-isbn-title-author-price
public class Book {
long isbn;
String title;
String author;
float price;
Book(long isbn,String title,String author,float price){
	this.isbn=isbn;
	this.title=title;
	this.author=author;
	this.price=price;
}
void displayDetails() {
System.out.println("ISBN of the book is "+isbn);
System.out.println("Book name is "+title);
System.out.println("Author of the book is "+author);
System.out.println("Price of the book is Rs. "+price);
}
void discountedPrice(int dp) {
float amount=price-price*dp/100;
System.out.println("The discounted amount to be paid is Rs. "+amount);
}
public static void main(String[] args) {
// TODO Auto-generated method stub
Book b=new Book(9780747532743L,"Harry Potter","J.K. Rowling",500);
b.displayDetails();
b.discountedPrice(20);
}
}

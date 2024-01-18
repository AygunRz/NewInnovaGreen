# Gruppe5_Fulton_Rzazade

<img width="943" alt="Screenshot 2024-01-17 at 12 27 04" src="https://github.com/linusfulton/InnovaGreen/assets/62143466/4ea86060-21e6-49d9-8eeb-e40bba9c2da1">

Das Projekt ist aus Frontend, Backend, und Datebank aufgebaut.

Das Frontend ist auf React aufgebaut, ein JavaScript-Framework, dass für die Erstellung von UIs verwenden wird. Diese werden hauptsächlich durch Komponenten aufgebaut, die in verschiedenen Views wiederverwenden werden können. Die zwei Komponenten sind "Navbar" und "Footer", da diese fast immer erscheinen. Pages sind AdminPage, CartPage, CheckoutPage, Home, Login, MyOrder, NewFood, Signup, SuccessPage und SupplierProducts.

State Management/LocalStorage wird verwenden, um mehrere Informationen zu speichern (zB. wer ist eingeloggt, welche Rolle, was liegt im Warenkorb, usw):
<img width="1176" alt="Screenshot 2024-01-17 at 12 48 05" src="https://github.com/linusfulton/InnovaGreen/assets/62143466/d7d896b2-4fea-4d09-b48a-5e2e6ce23e2c">
 
In dem Frontend ist ebenfalls eine GraphQL Integration eingebaut, die für Anfragen des Backend APIs zuständig ist.

Das Backend besteht aus Flask, einem Python Framework das für den Aufbau von Webservern verwendet wird. Weiters ist eine GraphQL API eingebaut. Diese ermöglicht es Anfragen zwischen Front- und Backend zu schicken. Im Backend gibt es auch die DB-Integration mit MongoDB.

MongoDB ist eine NoSQL Datenbank, die in Form von Collections Dokumenten speichert. Wir verwenden ein MongoDB Atlas Cluster, um auf unsere Daten zuzugreifen. Die DB "dataBase" enthält 4 Collections: "bankAccounts" (Felder: id, cardNumber, expiryDate, cvv, cardHolder, email, balance), "orders" (id, cartItems, totalPrice, orderDate, email, cardNumber), "products" (id, bezeichnung, verfallsdatum, standort, preis, leiferant) und "users" (id, name, email, address, password, role).

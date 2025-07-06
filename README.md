Warehouse Management System (Gudang App)
A comprehensive PHP-based warehouse management system for inventory tracking, stock management, and transaction processing.

📋 Features
User Management System with three role levels (Operator, Supervisor, Manager)
Dashboard with real-time inventory statistics
Interactive Charts for inventory movement analysis
Goods Reception with new product/location registration
Goods Release with stock validation
Stock Correction for inventory adjustments
Stock Reports with search functionality
Transaction History tracking all warehouse activities
User Profile Management with profile picture upload
Secure Authentication system
🖥️ System Requirements
PHP 7.4 or higher
MySQL 5.7 or higher
Web server (Apache, Nginx, etc.)
Modern web browser
🚀 Installation
Clone this repository to your web server directory:
Set up the database by importing the provided SQL script:
Configure database connection in database.php:
Ensure the web server has write permission to the upload directory.

Access the application at http://yourserver/gudang-app

🔑 Default Login Credentials
Username	Password	Role
admin	admin123	Manager
supervisor1	super123	Supervisor
operator1	oper123	Operator
👥 User Roles
Operator: Can receive and release goods
Supervisor: Can perform stock corrections and view reports
Manager: Full access including user management
📊 Database Structure
The system uses the following tables:

users: User authentication and role management
produk: Product catalog
lokasi_penyimpanan: Storage locations
stok: Current inventory
transaksi_penerimaan: Incoming goods
transaksi_pengeluaran: Outgoing goods
transaksi_koreksi: Stock corrections
audit_trail: System activity logs
📁 Directory Structure
📸 Screenshots


🔧 Technologies Used
PHP with PDO for database operations
MySQL database
Bootstrap for responsive design
Chart.js for interactive charts
Font Awesome for icons
JavaScript for client-side functionality
🛠️ Development Notes
For local development, we recommend using Laragon which provides an easy setup for PHP, MySQL, and Apache.
The system uses prepared statements for all database queries to prevent SQL injection.
User passwords are stored in plain text for this demo - implement proper password hashing for production use.
📝 To-Do / Future Improvements
Implement password hashing for security
Add barcode scanning functionality
Create mobile app integration
Add export functionality for reports
Implement email notifications
🤝 Contributing
Fork the repository
Create a feature branch: git checkout -b feature-name
Commit changes: git commit -am 'Add some feature'
Push to the branch: git push origin feature-name
Submit a pull request
📄 License
This project is licensed under the MIT License - see the LICENSE file for details.

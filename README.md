<!DOCTYPE html>
<html>
<head>
    <title>Digital Wallet (UPI-style) - Python Project</title>
</head>
<body>
    <h1>Digital Wallet (UPI-style) - Python Project</h1>
    <p>A command-line based digital wallet application that simulates UPI-style transactions with user authentication, transaction tracking, and reporting features.</p>

    <h2>📋 Table of Contents</h2>
    <ul>
        <li>Features</li>
        <li>Prerequisites</li>
        <li>Installation</li>
        <li>Usage</li>
        <li>Functionality</li>
        <li>Project Structure</li>
        <li>Data Storage</li>
        <li>Security Features</li>
    </ul>

    <h2>✨ Features</h2>

    <h3>🔐 Authentication & Account Management</h3>
    <ul>
        <li>User Registration: Create new accounts with unique usernames and 4-digit PINs</li>
        <li>Secure Login: PIN verification with 3-attempt limit and 5-second timeout</li>
        <li>PIN Management: Change PIN functionality with security validation</li>
    </ul>

    <h3>💰 Core Banking Operations</h3>
    <ul>
        <li>Deposit: Add money to account with transaction categorization</li>
        <li>Withdraw: Cash withdrawal with balance validation</li>
        <li>Balance Inquiry: Check current account balance</li>
        <li>Fund Transfer: Send money to other users (UPI-style)</li>
    </ul>

    <h3>📱 QR Code Payments</h3>
    <ul>
        <li>QR Generation: Create payment request payloads (JSON format)</li>
        <li>QR Payment: Process payments by scanning QR code payloads</li>
        <li>Transaction Recording: Automatic logging of QR transactions</li>
    </ul>

    <h3>📊 Reporting & Analytics</h3>
    <ul>
        <li>Transaction History: Complete transaction log with detailed information</li>
        <li>Category-wise Spending: Breakdown of expenses by category</li>
        <li>Monthly Summary: Inflow vs outflow analysis by month</li>
        <li>Top Payees: Ranking of most frequent payment recipients</li>
    </ul>

    <h2>🛠 Prerequisites</h2>
    <ul>
        <li>Python 3.8+</li>
        <li>Required packages:
            <ol>
                <li>rich - for progress bars and enhanced UI</li>
                <li>colorama - for colored terminal output</li>
                <li>inputimeout - for timed input sessions</li>
		<li>json - for interpreting json data</li>
		<li>datetime - for timestamps</li>
		<li>time - for timing the progress bar</li>
            </ol>
        </li>
    </ul>

    <h2>📥 Installation</h2>
    <ol>
        <li>Clone or download the project files</li>
        <li>Install required dependencies:
            <pre>pip install rich colorama inputimeout</pre>
        </li>
        <li>Run the application:
            <pre>python "Final Project.py"</pre>
        </li>
    </ol>

    <h2>🚀 Usage</h2>
    
    <h3>Main Menu Options:</h3>
    <ol>
        <li>Create Account - Register new user with username and PIN</li>
        <li>Login - Access existing account (3 attempts max)</li>
        <li>Exit - Close the application</li>
    </ol>

    <h3>User Dashboard Options:</h3>
    <ol>
        <li>Add Money - Deposit funds with category tracking</li>
        <li>Withdraw Money - Cash withdrawal</li>
        <li>Show Balance - Check current balance</li>
        <li>Transfer (UPI) - Send money to other users</li>
        <li>Generate QR - Create payment request</li>
        <li>Pay via QR - Process QR code payments</li>
        <li>Transaction History - View all transactions</li>
        <li>Report: Spent by Category - Category-wise expense analysis</li>
        <li>Report: Monthly In/Out - Monthly financial summary</li>
        <li>Report: Top Payees - Most frequent payment recipients</li>
        <li>Change PIN - Update security PIN</li>
        <li>Exit - Logout to main menu</li>
    </ol>

    <h2>💡 Functionality</h2>
    
    <h3>Transaction Categories</h3>
    <ul>
        <li>Food,
	<li>Travel,
	<li>Salary,
	<li>Bills,
	<li>Shopping, 
	<li>Education, 
	<li>Health, 
	<li>Others
	
    </ul>

    <h3>Transaction Types</h3>
    <ul>
        <li>deposit - Adding money to account</li>
        <li>withdraw - Cash withdrawal</li>
        <li>transfer_out - Sending money to others</li>
        <li>transfer_in - Receiving money from others</li>
        <li>qr_out - QR code payment sent</li>
        <li>qr_in - QR code payment received</li>
    </ul>

    <h3>Security Features</h3>
    <ul>
        <li>Session Timeout: 5-second limit for PIN entry</li>
        <li>Attempt Limiting: Maximum 3 failed login attempts</li>
        <li>PIN Validation: 4-digit numeric PIN requirement</li>
        <li>Balance Checks: Prevents overdrafts and invalid transactions</li>
    </ul>

    <h2>🗂 Project Structure</h2>
    <pre>
Digital Wallet/
├── Final Project.py          # Main application file
├── README.md                # This documentation
└── (Data stored in-memory)  # No external files required
    </pre>

    <h2>💾 Data Storage</h2>
    <p>The application uses an in-memory JSON structure with pre-loaded mock data for four demo accounts:</p>
    <p>Each account contains:</p>
    <ul>
        <li>PIN hash</li>
        <li>Current balance</li>
        <li>Transaction history with timestamps</li>
    </ul>

    <h2>🔒 Security Features</h2>
    <ul>
        <li>Timed Sessions: Automatic logout on PIN timeout</li>
        <li>Input Validation: Comprehensive error checking</li>
        <li>Transaction Integrity: Ensures sufficient funds before processing</li>
        <li>Unique Transaction IDs: Millisecond-based unique identifiers</li>
    </ul>

    <h2>🎨 UI/UX Features</h2>
    <ul>
        <li>Color-coded Output: Green for success, red for errors, yellow for information</li>
        <li>Progress Bars: Visual feedback for loading and saving operations</li>
        <li>Formatted Tables: Clean, aligned transaction displays</li>
        <li>ASCII Art Menus: Visually appealing interface</li>
    </ul>

    <p><strong>Note:</strong> This is a simulation project for educational purposes. All data is stored in memory and will be lost when the program terminates.</p>

    <p><strong>Guided by:</strong> Sanket Dodya (PythonGuruKool)<br>
    <strong>Developed by:</strong> Ayden Santhosh (PythonShishya)<br>
    <strong>Project Name:</strong> ApnaWallet - Digital Wallet Simulation</p>
</body>
</html>

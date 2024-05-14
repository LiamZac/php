<?php
// 1. Declare connection parameter variables
$servername = "localhost";
$username = "root";
$password = ""; // For XAMPP, the default password is empty
$dbname = "JustAnime3";

// 2. Call connection class: mysqli
$conn = new mysqli($servername, $username, $password, $dbname);

// 3. Test connection success or error: connect_error
if ($conn->connect_error) {
    die('<div class="alert alert-warning mt-3" role="alert">Connection Failed: ' . $conn->connect_error . '</div>');
} else {
    echo '<div class="alert alert-success mt-3" role="alert">Connection Successful</div>';
}
?>

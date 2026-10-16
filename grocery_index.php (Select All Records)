<?php require_once 'grocery_dbConfig.php'; ?>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Netherlands Grocery List</title>
</head>
<body>
    
    <h1>Grocery List</h1>
</body>
    <?php
    // Selecting ALL grocery items.
    $stmt = $pdo -> prepare("SELECT * FROM netherlands_grocery_items");
    if ($stmt->execute()) {
        $grocery = $stmt->fetchAll(PDO::FETCH_ASSOC); //using the fetchAll() method to retrieve all data from the database with $grocery as the variable to store the data.
        echo "<pre>";
        print_r($grocery); //using the print_r() and <pre> tags to display the data in a readable format. This will not show the data in table format but will be readable.
        echo "</pre>";
    } else { //will only show if the query fails to find any data or record in the database.
        echo "<p> No grocery items are found in the database.</p>";
    }
    ?>
</html>

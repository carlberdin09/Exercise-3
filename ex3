<?php

$filename = 'grp6_malinaomaryfeb_ex3.txt';


if (file_exists($filename)) 
{
    echo htmlspecialchars("The file '$filename' already exists.") . "<br>";
} 
else 
{
    
    $content = "Hello, this is a sample content written to the file.";
    
    
    if (file_put_contents($filename, $content) !== false) 
    {
        echo htmlspecialchars("The file '$filename' has been created and content has been written.") . "<br>";
    } 
    else 
    {
        echo htmlspecialchars("Failed to create the file '$filename'.") . "<br>";
    }
}


$fileContent = file_get_contents($filename);
if ($fileContent !== false) 
{
    echo "Content of the file '$filename':<br>";
    echo nl2br(htmlspecialchars($fileContent));
} 
else 
{
    echo htmlspecialchars("Failed to read the file '$filename'.") . "<br>";
}


$fileArray = file($filename);
if ($fileArray !== false) 
{
    echo "<br>File content as an array:<br>";
    print_r($fileArray);
} 
else 
{
    echo htmlspecialchars("Failed to read the file '$filename' as an array.") . "<br>";
}

?>

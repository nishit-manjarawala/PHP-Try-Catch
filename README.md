# PHP-Try-Catch

set_error_handler(function () {
    throw new Exception('Ach!');
});
try{
	echo 5/0;
}catch(Exception $e){
	echo"Try catch working now.";
}
restore_error_handler();

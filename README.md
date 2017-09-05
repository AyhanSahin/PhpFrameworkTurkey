# PhpFrameworkTurkey
       class demo extends controller {

control sayfası sayfa adı ile class adı aynı ;

class demo_sql extends load{

model sayfası yapısı sayfa adı uzerine _sql eklenerek class adı verilir.

temada herhangı bir kural yok.

conreolden model ve view  sayfalar 
model : $this->Model("user/demo");  // user klosoründeki demo.php model i çağırır.

      $data["class"] = $this->Model("user/demo"); 
      $this->View("user/header");
      $this->View("user/banka",$data);
      $this->View("user/footer");

oturum yonetimi
$this->session = $this->help("session");
$this->session->set("user_id","demo");
$this->session->get("user_id");

şifreleme 
$this->val->password; // get veya post ile gonderilen password anahtarı
$this->guvenlik()->sifrele_sha1($this->val->password);  

mail gondermek 

alıcı ve ek dosyalar dizi ile gondrilir.

$alici[0] = "xxx@xxx.com" ;
  self::sistem('mail')->sendmail($alici,$subject,$html,$ekdosyalar);


        
         

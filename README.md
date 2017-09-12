# PhpFrameworkTurkey
    class demo extends controller {
       
         function __construct($run) {
               parent::__construct($run);
         }
         
         function ayhan(){

             if($this->model("deneme")->kontrol($this->val->isim,$this->val->sifre)):
             return 1;
             else:return false;
             endif;
         
         }
          
       
       
   }


         

# Vücut Kitle Endeksi Hesaplama Uygulaması

Bu uygulamada kullanıcıdan metre olarak boy verisi ve kilogram olarak ağırlık verisi alıyoruz. Kullanıcı hesapla butonuna bastığı zaman
```
double boy = Double.parseDouble(txtHeight.getText());
double kilo = Double.parseDouble(txtWeight.getText());
double result = (kilo /(boy*boy));
```
komutu çalışarak vücut kitle endeksi hesabını yapar.
Daha sonrasında çıkan sonucu if bloklarıyla karşılaştırır. Uygun bulduğu sonucu arayüzde ilgili bölüme yazar. Çıkan sonuca göre kullanıcının
vücut kitle endeksini ve bu endeksin hangi duruma karşılık geldiğini yazar. Ek olarak çıkan sonuca göre kullanıcıya bir geri bildirimde bulunur.
```
if(result<18.5){
        lblResult.setText(result + ": ZAYIF");
        lblMessage.setText("Profesyonel destek almalısınız");
        }
        else if(result>18.5 && result< 24.9){
        lblResult.setText(result + ": NORMAL");
        lblMessage.setText("İyi durumdasınız");
        }
        else if(result>25 && result< 29.9){
        lblResult.setText(result + ": KİLOLU");
        lblMessage.setText("Kilonuza dikkat etmelisiniz");
        }
        else if(result>30 && result< 34.5){
        lblResult.setText(result + ": OBEZ");
        lblMessage.setText("Profesyonel destek almalısınz");
        }
        else{
        lblResult.setText(result + ": MORBİD OBEZ");
        lblMessage.setText("Profesyonel destek almalısınz");
        }
```        

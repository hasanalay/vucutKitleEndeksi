# Vücut Kitle Endeksi Hesaplama Uygulaması
Bu uygulama benim ilk arayüz uygulama deneyimim. Gördüğüm bir tutorial videosunun da yardımıyla ekstra özellikler de ekleyerek bu uygulamayı yaptım.

![1](https://user-images.githubusercontent.com/68869814/132590938-9154596f-662d-4a94-a526-7d85a58d7285.png)

Bu uygulamada kullanıcıdan metre olarak boy verisi ve kilogram olarak ağırlık verisi alıyoruz. Kullanıcı hesapla butonuna bastığı zaman

```
double boy = Double.parseDouble(txtHeight.getText());
double kilo = Double.parseDouble(txtWeight.getText());
double result = (kilo /(boy*boy));
```

komutu çalışarak vücut kitle endeksi hesabını yapar.
Daha sonrasında çıkan sonucu if bloklarıyla karşılaştırır. Uygun bulduğu sonucu arayüzde ilgili bölüme yazar. Çıkan sonuca göre kullanıcının
vücut kitle endeksini ve bu endeksin hangi duruma karşılık geldiğini yazar. Ek olarak çıkan sonuca göre kullanıcıya bir geri bildirimde bulunur.

![3](https://user-images.githubusercontent.com/68869814/132590980-b25f6e23-1495-46a4-a58c-46c1c8fdfbd6.png)
![5](https://user-images.githubusercontent.com/68869814/132590992-d1c72eef-8b8b-45b8-b9e2-aee6b2a23888.png)
![2](https://user-images.githubusercontent.com/68869814/132590970-4e00797c-954a-4c07-8453-303f7c35e594.png)

## Burada sonuca göre if yapısıyla text fieldlara neler yazacağımızı belirlemiş olduk. aşağıda kodu görebilirsiniz.
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

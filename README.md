# keylogger



İlk olarak, keyboard adlı bir modülü yüklememiz gerekecek. Terminal veya komut istemcisine gidin ve aşağıdaki komutu yazın:
$ pip install keyboard
Bu modül size klavyenizin tam kontrolünü sağlar, global olayları takip eder, kısayollar kaydeder, tuş vuruşlarını taklit eder ve çok daha fazlasını yapabilir. Ayrıca, oldukça küçük bir modüldür.

Bu Python betiği aşağıdakileri yapacaktır:

Arkaplanda tuş vuruşlarını dinler.
Herhangi bir tuşa basıldığında ve bırakıldığında, bu tuşu bir global string değişkenine ekleriz.
Her  dakikada bir, bu string değişkeninin içeriğini ya yerel bir dosyaya (FTP sunucusuna yüklemek veya Google Drive API'sini kullanmak için) ya da e-posta yoluyla raporlarız.
generate_encrypt_key metodu kullanıcının adını (kullanıcı adını) şifreleme anahtarı olarak kullanmak için getpass modülünü kullanır. Böylece her kullanıcının farklı bir şifreleme anahtarı olacaktır.

on_press ve on_release metotları kullanılarak tuş kayıtları alınır ve encrypt_log ve decrypt_log metotları ile kaydedilen veriler şifrelenir ve çözülür.

report_to_email metodu, şifrelenmiş logları e-posta ile göndermek için kullanılır. report_to_file metodu ise şifrelenmiş logları bir dosyaya kaydeder.

Ana programda, Keylogger sınıfı SEND_REPORT_EVERY değeriyle başlatılır ve start metodu çağrılarak keylogger başlatılır.

Kodun doğru çalışabilmesi için pynput kütüphanesini pip install pynput komutuyla kurmanız ve EMAIL_ADDRESS ve EMAIL_PASSWORD değişkenlerini kendi e-posta bilgilerinizle güncellemeniz gerekmektedir.



Yapacaklarınız sizin sorumluluğunuz altındadır bu içerik  eğitim amacıyla yazılmıştır.

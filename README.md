# Dogs vs Cats CNN Classifier
Bu repo, Akbank Derin Öğrenme Bootcamp projesi kapsamında hazırlanmıştır. Proje, Kaggle Dogs vs Cats veri seti kullanılarak, CNN tabanlı bir derin öğrenme modeli ile kedi-köpek görsellerinin sınıflandırılmasını amaçlamaktadır.
# Giriş
Bu çalışmada:
Kaggle’dan alınan Dogs vs Cats veri seti kullanıldı.
Veri önişleme adımları (görsellerin yeniden boyutlandırılması, normalizasyonu) uygulandı.
Eğitim sırasında data augmentation yöntemleri (çevirme, döndürme, yakınlaştırma vb.) kullanılarak modelin genelleme kabiliyeti artırıldı.
CNN tabanlı bir model sıfırdan inşa edildi, ayrıca hiperparametre optimizasyonu için KerasTuner HyperBand denemeleri yapıldı.
Notebook içerisinde sürecin teknik anlatımları Markdown hücrelerinde yer almaktadır.
# Metrikler
Modelin performans değerlendirmesi için şu metrikler kullanılmıştır:
Eğitim ve doğrulama için accuracy/loss grafikleri
Confusion Matrix ve classification report (precision, recall, F1-score)
Modelin nihai doğrulama başarımı: %77.80 accuracy ve F1: 0.7775
Ayrıca modelin karar mekanizmasını anlamak amacıyla Grad-CAM görselleştirmeleri eklenmiştir. Bu sayede modelin hangi bölgeleri dikkate alarak sınıflandırma yaptığı gözlemlenmiştir.
# Ekler
Grad-CAM görselleştirmeleri: Doğru ve hatalı sınıflandırmalardan örnekler.
Hiperparametre optimizasyonu: KerasTuner ile öğrenme oranı, batch size ve filtre sayıları denenmiş, en iyi konfigürasyon seçilmiştir.
İsteğe bağlı olarak, projenin gelecekte Streamlit veya benzeri araçlarla deploy edilmesi mümkündür.
# Sonuç ve Gelecek Çalışmalar
Model yüksek doğrulukla kedi ve köpekleri ayırt edebilmiştir. Ancak gelecekte:
Daha büyük ve dengeli veri setleriyle performans artırılabilir.
Transfer learning yöntemleri (ör. ResNet, EfficientNet) eklenerek daha yüksek doğruluk elde edilebilir.
Modelin web arayüzü üzerinden son kullanıcıya sunulması için Streamlit/Gradio gibi araçlar kullanılabilir.
# Linkler
https://www.kaggle.com/code/erayogunozdemir/dogs-vs-cats

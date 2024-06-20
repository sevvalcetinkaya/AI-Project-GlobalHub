# AI-Project-GlobalHub
 Bu proje, katılımcılara Fashion MNIST veri seti üzerinde farklı makine öğrenmesi ve derin öğrenme modelleri ile çalışma imkanı sunar. Verilerin ön işlenmesi, modellerin oluşturulması ve eğitilmesi, sonuçların çeşitli metriklerle değerlendirilmesi gibi adımları içerir. Her modelin performansı karşılaştırılarak, hangi algoritmanın veri seti üzerinde daha iyi sonuç verdiği analiz edilir.
 Katılımcılara çeşitli makine öğrenmesi ve derin öğrenme algoritmalarının nasıl kullanılacağını ve değerlendirileceğini öğretmektedir. Kullanılan Fashion MNIST veri seti, gerçek hayatta karşılaşılabilecek görüntü sınıflandırma problemlerine iyi bir örnektir. Makine öğrenmesi ve derin öğrenme modelleri arasındaki performans farkları ve bu farkların sebepleri üzerinde durmak, kullanıcılara model seçiminde dikkat edilmesi gereken noktalar hakkında değerli bilgiler sağlar.
Genel olarak, bu proje, yapay zeka ve makine öğrenmesi alanında temel bilgi ve deneyim kazanmak isteyenler için iyi bir başlangıç noktasıdır. İleride daha karmaşık ve büyük veri setleri üzerinde çalışarak, bu alandaki bilgi ve becerilerimizi daha da geliştirebiliriz.

Kullanılan Veri Seti: Fashion MNIST veri seti, kıyafet ve aksesuar resimlerinden oluşan bir veri setidir. Bu veri seti, her biri 28x28 piksel boyutunda gri tonlamalı görüntülerden oluşur. Toplamda 70,000 görüntü vardır; bunların 60,000'i eğitim ve 10,000'i test verisi olarak ayrılmıştır. Her görüntü, 0'dan 9'a kadar olan 10 farklı sınıftan birine aittir.

Analizler: KNN (K-Nearest Neighbors): Basit bir algoritma olmasına rağmen, sınıflandırma doğruluğu makul seviyedeydi ancak diğer metriklerde (precision, recall, f1-score) orta düzey performans gösterdi.
Decision Tree:: Aşırı uyum (overfitting) problemi nedeniyle test verisinde düşük performans gösterdi.
Random Forest: Birden fazla karar ağacını birleştirerek daha iyi genelleme yapar ve daha yüksek performans sağlar. Doğruluk ve diğer metriklerde iyi performans gösterdi, aşırı uyum problemini azalttı.

Kullanılan Yöntemler: 
Veri Ön İşleme
Normalize Etme: Veriler, [0, 255] aralığında piksel değerlerine sahip olduğu için, bu değerler [0, 1] aralığına normalize edildi. Bu, modelin daha hızlı ve verimli öğrenmesini sağlar.
Veri Düzleştirme: Makine öğrenmesi algoritmaları için veriler, 28x28 piksel boyutundaki görüntülerden 784 uzunluğunda düzleştirilmiş vektörlere dönüştürüldü.
Makine Öğrenmesi Modelleri
KNN (K-Nearest Neighbors): Komşuluk tabanlı bir sınıflandırıcı olup, eğitim verilerini bellekte tutar ve tahmin yaparken en yakın komşuları kullanır.
Decision Tree: Ağaç yapısı kullanarak veri setini sınıflandırır. Karar düğümleri ve yaprak düğümlerden oluşur.
Random Forest: Birden fazla karar ağacı oluşturur ve bunların sonuçlarını birleştirerek daha doğru ve kararlı tahminler yapar.

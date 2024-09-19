# ML-data-analysis
Kaggle linki: https://www.kaggle.com/code/barizz/aygaz-machine-learning-project

Projemizde Karar Ağacı ve Gaussian Naive Bayes modellerini kullandık. Genel değerlendirmeye baktığımızda karar ağacı modeli daha yüksek performans göstermiş görünüyor.

Naive Bayes algoritmaları, olasılıksal makine öğrenimi modelleridir ve sınıflar arasındaki bağımsız değişkenlik varsayımı ile çalışır. GNB, özelliklerin normal dağılım gösterdiği varsayımı ile Gaussian (sürekli veriler için) modelini kullanır. Yani, bir sınıfın özelliklerinin her biri bağımsız olarak bir Gaussian dağılımına göre dağılmış olarak ele alınır.

Avantajları:
Hızlı ve basit bir modeldir.
Çalıştırılması ve eğitimi genellikle çok az veriye ihtiyaç duyar.
Özellikle yüksek boyutlu verilerle iyi çalışır.

Dezavantajları:
Varsayımları nedeniyle gerçek hayatta, özelliklerin bağımsız olmadığı durumlarda performansı düşebilir.
Özellikle karmaşık veri setlerinde (bağımlı özellikler içeren) düşük performans gösterebilir.


Karar ağacı modeli, veriyi recursive partitioning ile belirli karar düğümleri üzerinden dallara ayırarak sınıflandırma yapan bir algoritmadır. Her düğüm bir karar sorusuna yanıt verir ve veri, belirli özelliklere dayalı olarak yapısal bir ağaç şeklinde sınıflara ayrılır.

Avantajları:
Karar verme süreci görsel olarak açıklanabilir ve kolayca anlaşılır.
Kategorik ve sürekli verilerle iyi çalışır.
Özellikler arasındaki etkileşimleri keşfetme yeteneği vardır.

Dezavantajları:
Ağaç derinleştikçe, model aşırı öğrenmeye (overfitting) eğilimli olabilir.
Dengeli olmayan veri setlerinde dengesiz sınıf dağılımı sorunları yaşayabilir.

Farkları ve Avantaj/Dezavantaj Karşılaştırması:

Temel Prensip:
GNB:
Olasılıksal model, bağımsız özellik varsayımı
Karar Ağacı:
Veri tabanlı karar süreci, veri özelliklerine dayalı dallar

Hız ve Basitlik:
GNB: 
Çok hızlı, az veri ile çalışabilir
Karar Ağacı:
Görece yavaş, büyüklük arttıkça hesaplama maliyeti artar

Varsayım:
GNB:
Özellikler birbirinden bağımsızdır
Karar Ağacı:
Veri hakkında varsayım yoktur

Overfitting Riski:
GNB:
Daha düşük
Karar Ağacı:
Daha Yüksek

Açıklanabilirlik:
GNB:
Daha az açıklanabilir
Karar Ağacı:
Açıklanabilir ve görselleştirilebilir

Performans:
GNB:
Bağımsız özelliklerde iyi performans
Karar Ağacı:
Karmaşık özellik etkileşimlerinde daha iyi

Karar Ağacı Modeli Neden Daha Yüksek Performans Gösterebilir?
Bir projede karar ağacı modeli, Gaussian Naive Bayes'e kıyasla daha yüksek performans gösterebilir, çünkü:

Özellikler bağımlıdır: GNB, özellikler arasındaki bağımsızlık varsayımına dayanır. Eğer bu varsayım geçerli değilse, GNB'nin performansı düşük olurken, karar ağaçları özellikler arasındaki bağımlılıkları yakalayabilir.

Veri karmaşıktır: Karar ağaçları, karmaşık özellik etkileşimlerini modelleyebilir ve veri üzerinde dallar ve düğümler aracılığıyla detaylı ayrımlar yapabilir.

Overfitting kontrolü: Eğer veri seti gürültülü ise, karar ağaçları iyi düzenlenmezse aşırı öğrenme eğiliminde olabilir, ancak pruning gibi teknikler kullanılarak bu sorun aşılabilir.

Hangi Tür Veri Setlerinde Kullanılmalı?

Gaussian Naive Bayes:
Özellikler arasında bağımsızlık varsayımı büyük ölçüde geçerliyse.
Özelliklerin sürekli (ve normal dağılım gösterdiği) veri setleri.
Büyük veri setlerinde hızlı bir şekilde sonuç almak gerektiğinde.

Karar Ağacı:
Özellikler arasında bağımlılıkların olduğu veri setlerinde.
Karmaşık veri yapıları ve özellik etkileşimleri olan veri setlerinde.
Verinin açıklanabilirliği ve görselleştirilebilirliğinin önemli olduğu durumlarda.

Her iki modelin de kullanılacağı durumlar veri setinin yapısına, bağımsızlık varsayımlarına ve model açıklığına göre değişir. Performans açısından, veri setinin özelliklerine göre seçim

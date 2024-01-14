# Django İle Web Projesi Oluşturma ve Temel Dosya Yapısı

## 1. Giriş

### Django Nedir?

Django, Python programlama dilini temel alan yüksek düzeyde bir web uygulama çerçevesidir. Web geliştirme süreçlerini hızlandırmak ve organize etmek amacıyla geliştirilen Django, özellikle karmaşık web uygulamaları ve siteleri oluşturmak için oldukça kullanışlıdır.

### Django'nun Avantajları Nelerdir?

1. **Hızlı Geliştirme:** Django, önceden oluşturulmuş birçok araç ve özelliği içerir, bu nedenle web uygulamalarını hızla geliştirmenize olanak tanır.

2. **Modüler Yapı:** Django, modüler bir yapı sunar ve bu nedenle web uygulamanızı parçalara ayırmanıza ve farklı bileşenleri kolayca yeniden kullanmanıza olanak tanır.

3. **Veritabanı Bağımsızlığı:** Django, birçok farklı veritabanı sistemini destekler ve uygulamanızı farklı veritabanlarına kolayca taşımanıza olanak tanır.

4. **MVT Tasarım Deseni:** Django, Model-View-Template (MVT) tasarım desenini kullanır, bu da veritabanı işlemlerini, kullanıcı arayüzünü ve şablonları daha net bir şekilde ayrıştırmanıza olanak tanır.

5. **Otomatik Yönetim Arayüzü:** Django, veritabanı yönetimi için otomatik bir yönetim arayüzü sağlar.

6. **Güvenlik:** Django, güvenli bir şekilde web uygulamaları geliştirmenize yardımcı olur ve kullanıcı kimlik doğrulama, oturum yönetimi gibi güvenlik önlemleri sunar.

7. **URL Yönlendirmeleri:** Django, URL yönlendirmelerini ve rota tanımlamalarını kolayca yönetmenizi sağlar.

8. **Dökümantasyon ve Topluluk:** Django'nun kapsamlı bir dökümantasyonu ve büyük bir geliştirici topluluğu vardır.

## 2. Django Kurulumu

### Python ve pip Kurulumu

- Python'un [resmi web sitesinden](https://www.python.org/downloads/) en son sürümünü indirip kurun.

- Pip kontrolü için terminal veya komut istemcisine `pip --version` komutunu girin.

### Django'nun Pip ile Kurulumu

- Django'yu pip aracılığıyla kurmak için terminal veya komut istemcisine `pip install django` komutunu girin.

- Kurulumun başarıyla tamamlandığını doğrulamak için `django-admin --version` komutunu kullanın.

## 3. Temel Dosya Yapısı

### Django Projesinin Ana Dizini

- Projeyi oluşturduktan sonra ana dizinde şu dosyaları bulabilirsiniz:

  - **`settings.py`:** Proje ayarlarının yapılandırıldığı dosya.
  
  - **`urls.py`:** URL yönlendirmelerinin bulunduğu dosya.
  
  - **`wsgi.py`:** WSGI uyumlu web sunucusu arayüzü dosyası.
  
  - **`asgi.py`:** ASGI uyumlu asenkron web sunucusu arayüzü dosyası.
  
  - **`manage.py`:** Proje yönetim komutlarının bulunduğu dosya.

## 4. Uygulama Oluşturma

### Django Uygulamaları Hakkında Genel Bilgi

- Django uygulamaları, web uygulamasının farklı bölümlerini ve işlevselliğini düzenleyen modüler bileşenlerdir.

### Temel Komutlar

- Yeni bir Django uygulaması oluşturmak için terminal veya komut istemcisine `python manage.py startapp myapp` komutunu girin.

- Oluşturulan uygulama klasörü içinde `models.py`, `views.py`, `urls.py`, `admin.py` gibi dosyalar bulunur.

- Uygulamayı projeye eklemek için projenin `settings.py` dosyasındaki `INSTALLED_APPS` listesine uygulamanın adını ekleyin.

## 5. Temel Dosya Yapısı (Uygulama Seviyesi)

### Uygulama Dizinleri

- Uygulama klasörü içinde genellikle şu ana dizinler bulunur:

  - **`migrations/`:** Veritabanı değişikliklerini yönetmek için kullanılan klasör.
  
  - **`templates/`:** HTML şablonlarını içeren klasör.
  
  - **`static/`:** Uygulama özgü statik dosyaların (CSS, JavaScript, resimler) bulunduğu klasör.

### Dosya Açıklamaları

- **`models.py`:** Veritabanı modellerini tanımladığınız dosya.

- **`views.py`:** Görünüm fonksiyonlarını içeren dosya.

- **`urls.py`:** URL yönlendirmelerini belirlediğiniz dosya.

- **`admin.py`:** Django admin paneli yapılandırmasını yaptığınız dosya.

- **`templates/`:** HTML şablonlarını içeren klasör.

- **`static/`:** Statik dosyaların (CSS, JS, vb.) bulunduğu klasör.

Bu temel dosya yapısı, bir Django uygulamasının organizasyonunu ve işlevselliğini düzenler. Her uygulama, projenin bir parçası olarak projenin ana dizinine eklenir ve projenin daha büyük bir bütün olarak yönetilmesine olanak tanır.

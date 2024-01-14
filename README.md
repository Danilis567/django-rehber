Django, Python tabanlı bir web framework'üdür ve hızlı bir şekilde güçlü web uygulamaları geliştirmenizi sağlar. Django projenizi başlatmak ve temel dosya yapısını anlatan bir makale şu başlıkları içerebilir:

1\. Giriş
---------

\- Django nedir?

\- Django'nun avantajları nelerdir?

Django, Python programlama dilini temel alan yüksek düzeyde bir web uygulama çerçevesidir. Web geliştirme süreçlerini hızlandırmak ve organize etmek amacıyla geliştirilen Django, özellikle karmaşık web uygulamaları ve siteleri oluşturmak için oldukça kullanışlıdır. Aşağıda Django'nun temel özellikleri ve işlevleri hakkında daha fazla bilgi bulabilirsiniz:

1\. **Hızlı Geliştirme:** Django, önceden oluşturulmuş birçok araç ve özelliği içerir, bu nedenle web uygulamalarını hızla geliştirmenize olanak tanır. Böylece geliştiriciler daha fazla zamanlarını işlevselliği eklemeye odaklayabilirler.

2\. **Modüler Yapı:** Django, modüler bir yapı sunar ve bu nedenle web uygulamanızı parçalara ayırmanıza ve farklı bileşenleri kolayca yeniden kullanmanıza olanak tanır. Django uygulamalarınızı küçük, bağımsız uygulama parçalarına bölebilirsiniz.

3\. **Veritabanı Bağımsızlığı:** Django, birçok farklı veritabanı sistemini destekler (örneğin PostgreSQL, MySQL, SQLite, Oracle) ve uygulamanızı farklı veritabanlarına kolayca taşımanıza olanak tanır.

4\. **MVC (Model-View-Controller) Tasarım Deseni:** Django, Model-View-Controller (MVC) tasarım deseni yerine Model-View-Template (MVT) tasarım desenini kullanır. Bu, veritabanı işlemlerini, kullanıcı arayüzünü ve şablonları daha net bir şekilde ayrıştırmanıza olanak tanır.

5\. **Otomatik Yönetim Arayüzü:** Django, veritabanı yönetimi için otomatik bir yönetim arayüzü sağlar. Bu, veritabanınızı düzenlemenizi, verileri eklemenizi, güncellemenizi veya silmenizi kolaylaştırır.

6\. **Güvenlik:** Django, güvenli bir şekilde web uygulamaları geliştirmenize yardımcı olur. Özellikle kullanıcı kimlik doğrulama, oturum yönetimi ve diğer güvenlik önlemleri için yerleşik çözümler sunar.

7\. **URL Yönlendirmeleri:** Django, URL yönlendirmelerini ve rota tanımlamalarını kolayca yönetmenizi sağlar, böylece web uygulamanızın URL'lerini düzenleyebilir ve yeniden yapılandırabilirsiniz.

8. **Dökümantasyon ve Topluluk:** Django'nun kapsamlı bir dökümantasyonu ve büyük bir geliştirici topluluğu vardır. Bu, sorularınıza cevap bulmanız ve projelerinizi geliştirmeniz için faydalı kaynaklar sunar.

Django, büyük ölçekli ve karmaşık web uygulamaları geliştirmek için güçlü bir araçtır ve bu framework sayesinde temel web geliştirme görevlerini daha kolay ve verimli bir şekilde gerçekleştirebilirsiniz.

2\. Django Kurulumu
-------------------

\- Python ve pip kurulumu

\- Django'nun pip ile kurulumu

1.  **Python İndirme ve Kurulumu:**
    
    *   İlk olarak, bilgisayarınızda Python'un yüklü olduğundan emin olun. Python'ın resmi web sitesinden en son sürümü indirebilir ve kurabilirsiniz. Python 3 önerilir: [Python İndirme Sayfası](https://www.python.org/downloads/ "https://www.python.org/downloads/")
        
    
2.  **Pip Kontrolü:**
    
    *   Pip (Python Package Index) Python paketlerini yönetmek için kullanılır. Python'un kurulumu sırasında pip'in otomatik olarak yüklenip yüklenmediğini kontrol edin. Komut satırında aşağıdaki komutu çalıştırarak pip sürümünü kontrol edebilirsiniz:`pip --version`
        
    
3.  **Django Kurulumu:**
    
    *   Pip'i kullanarak Django'yu kurabilirsiniz. Komut satırında aşağıdaki komutu çalıştırarak en son Django sürümünü kurun:`pip install django   `
        
    
    Bu komut, Django'nun en son sürümünü Python ortamınıza indirecek ve kuracaktır.
    
4.  **Kurulumu Doğrulama:**
    
    *   Django'nun başarıyla kurulup kurulmadığını doğrulamak için aşağıdaki komutu kullanabilirsiniz:`django-admin --version`
        
    
    Bu komut, Django'nun sürümünü göstermelidir.
    

Django başarıyla kurulduğunda, web uygulamaları geliştirmeye başlamak için hazırsınız demektir. Django'nun güçlü yeteneklerinden ve ayrıntılı dökümantasyonundan yararlanarak web projelerinizi oluşturabilir ve yönetebilirsiniz. Kurulum tamamlandıktan sonra, `django-admin` veya `django-admin.py` kullanarak Django komutlarını kullanabilirsiniz. Örneğin, yeni bir Django projesi oluşturmak için `django-admin startproject myproject` komutunu kullanabilirsiniz. Projenizi oluşturduktan sonra, web uygulamanızı geliştirmeye başlamak için Django belgelerini incelemek iyi bir başlangıç olacaktır.

5\. Temel Dosya Yapısı
----------------------

\- Django projesinin ana dizini

\- \`settings.py\`: Proje ayarları

\- \`urls.py\`: URL Yönlendirmeleri

\- \`wsgi.py\`: Web sunucusu arayüzü

\- \`asgi.py\`: Asenkron web sunucusu arayüzü

\- \`manage.py\`: Proje yönetim komutları

1.  **Django Projesinin Ana Dizini:**
    
    *   Django projesi oluşturulduğunda, bu projenin ana dizini oluşturulur. Projenin adına göre adlandırılmış bir klasördür. Bu dizin, projenin tüm bileşenlerini içerir ve projenin ana kütüphanesidir.
        
    
2.  `settings.py`**: Proje Ayarları:**
    
    *   `settings.py`, Django projesinin temel ayarlarının yapılandırıldığı dosyadır. Bu dosya içinde veritabanı bağlantısı, dil ayarları, zaman dilimi, statik dosyaların konumu, uygulama listesi ve daha birçok projeye özgü ayar bulunur. Projenin tüm ayarlarını burada yapılandırabilirsiniz.
        
    
3.  `urls.py`**: URL Yönlendirmeleri:**
    
    *   `urls.py`, projenin URL yapılandırmasını belirlediğiniz dosyadır. Bu dosya, gelen istekleri doğru görünüme yönlendirmek için URL desenleri ile görünüm fonksiyonlarını eşler. Bu sayede projenizin hangi URL'lerin hangi görünümlere yönlendirileceğini tanımlayabilirsiniz.
        
    
4.  `wsgi.py`**: Web Sunucusu Arayüzü:**
    
    *   `wsgi.py`, Django projesini Web Server Gateway Interface (WSGI) uyumlu bir web sunucusuna entegre etmek için kullanılır. WSGI, Python web uygulamalarının web sunucuları ile iletişim kurmasını sağlayan bir standart arayüzdür. Bu dosya, Django projenizi WSGI uyumlu bir sunucuya dağıtmak için kullanılır.
        
    
5.  `asgi.py`**: Asenkron Web Sunucusu Arayüzü:**
    
    *   `asgi.py`, Django projesini asenkron web sunucusu arayüzü (ASGI) uyumlu bir sunucuya entegre etmek için kullanılır. ASGI, Django'nun asenkron istekleri ve WebSocket bağlantılarını desteklemesine olanak tanır. Bu dosya, Django projelerini asenkron özelliklerle kullanmak istediğinizde kullanılır.
        
    
6.  `manage.py`**: Proje Yönetim Komutları:**
    
    *   `manage.py`, Django projesi ile etkileşimde bulunmanıza ve çeşitli proje yönetim komutlarını çalıştırmanıza olanak tanır. Bu komutlar aracılığıyla yeni uygulamalar oluşturabilir, veritabanını yönetebilir, geliştirme sunucusunu başlatabilir, yönetici kullanıcı oluşturabilir ve daha fazlasını yapabilirsiniz.
        
    

Django'nun temel dosya yapısı, projenizin temel bileşenlerini düzenler ve projenizi kolayca yönetmenize yardımcı olur. Bu dosyaları düzgün bir şekilde yapılandırarak, Django ile web projelerinizi geliştirmeye başlayabilirsiniz. Proje geliştikçe, bu dosyaların içeriğini özelleştirmeniz ve yeni uygulamalar eklemeniz gerekecektir.

6\. Uygulama Oluşturma
----------------------

\- Django uygulamaları hakkında genel bilgi

\- Temel komutlar: \`python manage.py startapp myapp\`

  
Django uygulamaları, bir Django projesinin modüler bileşenleridir ve proje içinde farklı işlevselliği ve veri modellemesini temsil ederler. Her Django projesi, bir veya daha fazla uygulama içerebilir. Aşağıda Django uygulamaları hakkında genel bilgi ve uygulama oluşturma adımlarını bulabilirsiniz:

**Django Uygulamaları Hakkında Genel Bilgi:**

*   Django uygulamaları, web uygulamanızın farklı bölümlerini ve işlevselliğini düzenlemek ve gruplandırmak için kullanılır. Her uygulama, kendi veritabanı modellerini, görünüm fonksiyonlarını, URL yönlendirmelerini ve şablon dosyalarını içerebilir. Bu, büyük ve karmaşık projelerin daha iyi yönetilmesine olanak tanır.
    
*   Her Django uygulaması, projenin ana dizini içinde bir klasör olarak oluşturulur. Bu klasör, uygulamanın adını taşır ve içinde bir dizi dosya ve alt klasör bulunur.
    

**Django Uygulaması Oluşturma Adımları:**

1.  **Uygulama Oluşturma Komutu:**
    
    *   Yeni bir Django uygulaması oluşturmak için aşağıdaki komutu kullanabilirsiniz. "myapp" kısmını oluşturmak istediğiniz uygulamanın adıyla değiştirin.
        
    *   `python manage.py startapp myapp   `
        
    
2.  **Uygulama Klasörü Oluşturulur:**
    
    *   Komutu çalıştırdığınızda, belirttiğiniz ad ile yeni bir uygulama klasörü oluşturulur. Bu klasörün adı "myapp" ya da sizin belirlediğiniz ad olacaktır.
        
    
3.  **Uygulama Dosyaları:**
    
    *   Oluşturulan uygulama klasörü içinde, uygulamanızla ilgili temel dosyalar ve alt klasörler bulunur. Bu dosyalar şunlar içerebilir:
        
        *   `models.py`: Veritabanı modelleri için kullanılır.
            
        *   `views.py`: Görünüm fonksiyonları için kullanılır.
            
        *   `urls.py`: Uygulama URL yönlendirmeleri için kullanılır.
            
        *   `admin.py`: Django admin paneli yapılandırması için kullanılır.
            
        *   `apps.py`: Uygulama yapılandırması ve ayarları için kullanılır.
            
        *   `tests.py`: Testlerin tanımlandığı dosya.
            
        *   `migrations/`: Veritabanı değişikliklerinin takip edildiği klasör.
            
        *   `templates/`: HTML şablonları için kullanılır.
            
        *   `static/`: Uygulama özgü statik dosyalar için kullanılır.
            
        
    
4.  **Uygulamanın Projeye Eklenmesi:**
    
    *   Yeni oluşturulan uygulamayı Django projesine eklemek için, projenin ayar dosyası olan `settings.py` içindeki `INSTALLED_APPS` listesine uygulamanın adını eklemelisiniz.
        
    *   `INSTALLED_APPS = [   # ...'myapp',   ]`
        
    

Bu adımları takip ederek yeni bir Django uygulaması oluşturabilir ve projenize ekleyebilirsiniz. Uygulama içinde veritabanı modelleri tanımlayabilir, görünümler ve şablonlar oluşturabilir ve projenizin farklı bölümlerini düzenleyebilirsiniz.

7\. Temel Dosya Yapısı (Uygulama Seviyesi)
------------------------------------------

\- Uygulama dizinleri

\- \`models.py\`: Veritabanı modelleri

\- \`views.py\`: Görünüm fonksiyonları

\- \`urls.py\`: Uygulama URL yönlendirmeleri

\- \`admin.py\`: Django admin paneli yapılandırması

\- \`templates/\`: HTML şablonları

\- \`static/\`: Statik dosyalar (CSS, JS, vb.)

Django uygulamaları, her uygulamanın kendi işlevselliğini düzenlediği ve projenizin modülerliğini artırdığı bölümlerdir. İşte bir Django uygulamasının temel dosya yapısı ve bu dosyaların işlevleri:

1.  **Uygulama Dizinleri:**
    
    *   Django uygulaması, genellikle şu ana dizinlere sahiptir:
        
        *   `myapp/` (örneğin, uygulamanın adı): Uygulamanın ana dizini.
            
        *   `migrations/`: Veritabanı değişikliklerini yönetmek için kullanılan klasör.
            
        *   `templates/`: HTML şablonlarını içeren klasör.
            
        *   `static/`: Uygulama özgü statik dosyaların (CSS, JavaScript, resimler) bulunduğu klasör.
            
        
    
2.  `models.py`**: Veritabanı Modelleri:**
    
    *   `models.py`, uygulama tarafından kullanılan veritabanı tablolarının (modellerin) tanımlandığı dosyadır. Bu modeller, verilerin nasıl saklandığını ve yönetildiğini tanımlar. Django'nun ORM (Object-Relational Mapping) kullanarak veritabanı işlemlerini gerçekleştirmenize olanak tanır.
        
    
3.  `views.py`**: Görünüm Fonksiyonları:**
    
    *   `views.py`, uygulamanın kullanıcı isteklerine nasıl yanıt vereceğini belirleyen görünüm fonksiyonlarını içerir. Her görünüm işlevi, bir HTTP isteği alır, verileri işler ve bir HTTP yanıtı döndürür. Bu dosya, web uygulamanızın işlevselliğini uygular.
        
    
4.  `urls.py`**: Uygulama URL Yönlendirmeleri:**
    
    *   `urls.py`, uygulamanın URL yapılandırmasını belirler. Gelen URL isteklerini hangi görünümlere yönlendireceğinizi ve nasıl işleyeceğinizi tanımlar. URL yönlendirmeleri, projenin ana `urls.py` dosyası tarafından dahil edilir.
        
    
5.  `admin.py`**: Django Admin Paneli Yapılandırması:**
    
    *   `admin.py`, Django admin panelini yapılandırmak için kullanılır. Admin paneli, projenizin veritabanı ile etkileşim kurmanıza ve verileri yönetmenize olanak tanır. Veritabanı modellerini burada admin paneline kaydeder ve özelleştirirsiniz.
        
    
6.  `templates/`**: HTML Şablonları:**
    
    *   `templates/` klasörü, uygulamanın kullanıcı arayüzünün HTML şablonlarını içerir. Django, şablonlar ile veritabanı verilerini birleştirmenize ve dinamik web sayfaları oluşturmanıza olanak tanır. Şablonlar, kullanıcıların projenizin içeriğini görüntülediği yerdir.
        
    
7.  `static/`**: Statik Dosyalar (CSS, JS, vb.):**
    
    *   `static/` klasörü, uygulamanın statik dosyalarını (CSS, JavaScript, resimler vb.) içerir. Bu dosyalar, web sayfasının tasarımını ve işlevselliğini geliştirmek için kullanılır. Django, bu statik dosyaları sunucu üzerinden sunar.
        
    

Bu temel dosya yapısı, bir Django uygulamasının organizasyonunu ve işlevselliğini düzenler. Her uygulama, projenin bir parçası olarak projenin ana dizinine eklenir ve projenin daha büyük bir bütün olarak yönetilmesine olanak tanır. Uygulamalar, farklı işlevselliği ve bileşenleri kolayca tanımlamanıza ve gruplandırmanıza yardımcı olur.

8.Veritabanı Ayarları
---------------------

\- Veritabanı bağlantısı yapılandırma

\- Django ORM (Object-Relational Mapping) kullanımı

Django, veritabanı bağlantısı ve yönetimi için güçlü bir araç olan Django ORM (Object-Relational Mapping) ile birlikte gelir. İşte Django'da veritabanı ayarlarını yapılandırma ve Django ORM kullanma hakkında temel bilgiler:

**1\. Veritabanı Bağlantısı Yapılandırma:**

Django projenizdeki veritabanı bağlantısını yapılandırmak için `settings.py` dosyasını kullanırsınız. Bu dosyada `DATABASES` ayarı altında veritabanı bağlantısı tanımlanır. Aşağıda, `settings.py` dosyasındaki tipik veritabanı ayarlarını görüyorsunuz

```python
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.sqlite3',  # Veritabanı motoru
        'NAME': os.path.join(BASE_DIR, 'db.sqlite3'),  # Veritabanı dosyasının yolu
    }
}
```

*   `'ENGINE'`: Kullanmak istediğiniz veritabanı motorunu belirtir. Örnek olarak SQLite, PostgreSQL, MySQL veya Oracle gibi veritabanı motorlarını seçebilirsiniz.
    
*   `'NAME'`: Veritabanının fiziksel dosya yolu veya veritabanı adıdır. SQLite kullanırken, dosyanın yolunu belirtirsiniz.
    

**2\. Django ORM (Object-Relational Mapping) Kullanımı:**

Django ORM, veritabanı işlemlerini Python nesneleri ve sorguları ile yönetmenize olanak tanır. İşte bazı Django ORM kullanım örnekleri:

*   **Model Tanımlama:**  
    Django ORM'de veritabanı tablolarını Python sınıfları ile tanımlarsınız. Örnek bir model tanımı:
    
```
from django.db import models
    class Author(models.Model):
    name = models.CharField(max_length=100)
    birth_date = models.DateField()
```
    
*   **Yeni Veri Ekleme:**  
    Yeni veri eklemek için modeli kullanabilirsiniz:
    
```
new_author = Author(name="J.K. Rowling",birth_date="1965-07-31")
new_author.save()
```
    
*   **Veri Sorgulama:**  
    Veritabanından veri sorgulamak için Django ORM sorgularını kullanabilirsiniz:
    
```
authors = Author.objects.filter(name="J.K. Rowling")
```
    
*   **Veri Güncelleme:**  
    Veritabanındaki verileri güncellemek için modeli kullanabilirsiniz:
    
```
author = Author.objects.get(name="J.K. Rowling")
author.name = "Joanne Rowling"
author.save()
```
    
*   **Veri Silme:**  
    Verileri silmek için Django ORM'yi kullanabilirsiniz:

```
author = Author.objects.get(name="Joanne Rowling")
author.delete()
``` 
    

Django ORM, veritabanı işlemlerini Python nesneleri ve sorguları ile yapmanıza olanak tanır ve veritabanı bağlantısı için yapılandırma işlemlerini `settings.py` dosyası içinde kolayca yapabilirsiniz. Bu, veritabanı işlemlerini yönetmeyi daha kolay ve veritabanı bağlantısını esnek hale getirir.

9\. URL Yönlendirmeleri
-----------------------

\- URL yönlendirmeleri ve \`urls.py\` kullanımı

\- Parametreli URL yönlendirmeleri

Django'da URL yönlendirmeleri, gelen HTTP isteklerini doğru görünümlere yönlendirmenizi sağlar. URL yönlendirmelerini `urls.py` dosyaları içinde tanımlayarak yapılandırırsınız. İşte URL yönlendirmeleri ve `urls.py` kullanımı hakkında temel bilgiler:

**1\. URL Yönlendirmeleri ve** `urls.py` **Kullanımı:**

*   Django projelerinizde URL yönlendirmeleri, her uygulama için ayrı `urls.py` dosyalarında tanımlanır. Her uygulamanın `urls.py` dosyası, o uygulamanın URL yapılandırmasını belirler.
    
*   Ana projenin `urls.py` dosyası, tüm uygulamaların URL yapılandırmalarını içeren ana URL yapılandırmasını belirler.
    

Örnek bir `urls.py` dosyası:

```
from django.urls import path
from . import views

urlpatterns = [
    path('', views.home, name='home'),         # Anasayfa
    path('about/', views.about, name='about'),  # Hakkında sayfası
    path('contact/', views.contact, name='contact'),  # İletişim sayfası
]

```

*   Yukarıdaki örnekte, her yol (URL) bir görünüm fonksiyonu ile ilişkilendirilir. Örneğin, boş bir yol (`''`) ana sayfayı temsil eder ve `home` adlı bir görünüm fonksiyonuna yönlendirilir.
    

**2\. Parametreli URL Yönlendirmeleri:**

Django'da URL yönlendirmeleri, parametreli yolları destekler. Bu, dinamik verileri URL içinde yakalamak ve işlemek için kullanışlıdır. Örneğin, belirli bir kullanıcının profil sayfasını görüntülemek için parametreli URL yönlendirmeleri kullanabilirsiniz.

Örnek parametreli URL yönlendirmesi:

```
from django.urls import path
from . import views

urlpatterns = [
    path('profile/<int:user_id>/', views.user_profile, name='user_profile'),
]

```

*   Yukarıdaki örnekte, `<int:user_id>` ile tanımlanan kısım, bir kullanıcının kimlik numarasını belirtir. Bu, URL içindeki bir sayıyı yakalamak için kullanılır ve bu sayı, `user_profile` görünüm fonksiyonuna iletilir.
    
*   Görünüm fonksiyonunda, parametre olarak `user_id` kullanılabilir ve bu sayede kullanıcının profili ilgili kimlik numarasına göre görüntülenebilir.
    

Django, URL yönlendirmelerini tanımlarken çeşitli özel dize düzenlemeleri ve parametre yakalama yöntemleri sunar. Bu, web uygulamanızın URL'lerini özelleştirmenize ve istediğiniz dinamik verilere erişmenize olanak tanır.

10\. Görünümler (Views)
-----------------------

\- Görünüm fonksiyonları oluşturma

\- HTTP istekleri ve cevapları

Django'da görünümler (views), HTTP isteklerini alır, işler ve HTTP cevaplarını döndürür. Görünüm fonksiyonları, web uygulamanızın işlevselliğini yönlendirmek ve dinamik web sayfaları oluşturmak için kullanılır. İşte görünüm fonksiyonlarını oluşturma ve HTTP istekleri ile cevapları işleme hakkında temel bilgiler:

**1\. Görünüm Fonksiyonları Oluşturma:**

Görünüm fonksiyonlarını oluşturmak için Django'da Python fonksiyonlarını kullanırsınız. Her görünüm fonksiyonu, bir veya daha fazla HTTP isteği türünü (GET, POST, vb.) işlemek için tanımlanır. İşte bir örnek görünüm fonksiyonu:

`from django.http import HttpResponse      def home(request):   return HttpResponse("Ana Sayfa")   `

Yukarıdaki örnek, "home" adlı bir görünüm fonksiyonu tanımlar. Bu görünüm, gelen HTTP GET isteğini işler ve "Ana Sayfa" metinli bir HTTP yanıtı döndürür.

**2\. HTTP İstekleri ve Cevapları:**

*   Django'da HTTP istekleri ve cevapları, `request` ve `response` nesneleri kullanılarak işlenir.
    
*   `request` nesnesi, gelen HTTP isteğini temsil eder ve bu nesne içinde isteğin detayları, parametreleri, kullanıcı kimlik doğrulama bilgileri ve daha fazlası bulunur.
    
*   `response` nesnesi, HTTP yanıtını temsil eder ve bu nesne içinde yanıtın içeriği, başlıkları ve diğer özellikleri bulunur.
    

Örnek bir görünüm fonksiyonunda HTTP isteği ve cevabının kullanımı:
```
from django.http import HttpResponse

def greet_user(request, user_name):
    message = f"Merhaba, {user_name}"
    return HttpResponse(message)
```

Yukarıdaki örnekte, "greet\_user" adlı bir görünüm fonksiyonu tanımlanmıştır. Bu görünüm, URL'den yakalanan `user_name` parametresini alır ve bu parametreyi kullanarak bir "Merhaba" yanıtı oluşturur. Oluşturulan yanıt, `HttpResponse` nesnesi ile döndürülür.

Django, HTTP isteklerini işlemek ve HTTP cevapları oluşturmak için birçok farklı nesne ve araç sunar. Görünüm fonksiyonları, web uygulamanızın işlevselliğini ve kullanıcı arayüzünü kontrol etmek için önemli bir rol oynar.

11\. HTML Şablonları
--------------------

\- Django şablonları ve HTML kullanımı

\- Şablon değişkenleri ve döngüler

Django'da HTML şablonları, web sayfalarını oluşturmanızı ve dinamik içerikleri sunmanızı sağlayan önemli bir özelliktir. Şablonlar, HTML belgelerine eklenen özel etiketler ve dil yapıları kullanılarak oluşturulur. İşte Django şablonları ve HTML kullanımı hakkında temel bilgiler:

**1\. Django Şablonları ve HTML Kullanımı:**

Django şablonları, HTML belgelerinin içine eklenen özel etiketler ve ifadeler ile oluşturulur. Bu özel etiketler ve ifadeler, dinamik verileri veya döngüler gibi Django uygulamanızın işlevselliğini temsil eder.

*   `{% %}`: Bu etiketler, kontrol yapıları ve şablon blokları için kullanılır. Örneğin, `{% if kullanici_girisli %} ... {% endif %}` ile bir koşul ifadesi tanımlanabilir.
    
*   `{{ }}`: Bu etiketler, şablon değişkenlerini içerir. Değişkenler, şablon ile iletişim kurmanızı sağlar. Örneğin, `Merhaba, {{ kullanici_isim }}` ile bir değişken içeriği görüntülenir.
    
*   `{# #}`: Bu etiketler, açıklamalar için kullanılır ve şablonda belgelendirmeler eklemek için kullanışlıdır.
    

Örnek bir Django şablonu:

```
<!DOCTYPE html>
<html>
<head>
    <title>{{ sayfa_basligi }}</title>
</head>
<body>
    <h1>Merhaba, {{ kullanici_isim }}</h1>

    {% if kullanici_girisli %}
        <p>Kullanıcı giriş yapmış.</p>
    {% else %}
        <p>Kullanıcı giriş yapmamış.</p>
    {% endif %}

    <ul>
        {% for sehir in sehirler %}
            <li>{{ sehir }}</li>
        {% endfor %}
    </ul>
</body>
</html>
```

Yukarıdaki örnekte, Django şablonları içinde değişkenler (`{{ sayfa_basligi }}`, `{{ kullanici_isim }}`), koşul ifadeleri (`{% if kullanici_girisli %}`), ve döngüler (`{% for sehir in sehirler %}`) kullanılmıştır.

**2\. Şablon Değişkenleri ve Döngüler:**

Django şablonlarında değişkenler, verilerin dinamik olarak görüntülenmesini sağlar. Değişkenler, `{{ }}` etiketleri içinde tanımlanır ve görünüm fonksiyonlarından gelen verileri temsil eder.

Döngüler, listedeki veya sorgudan dönen verileri şablonda görüntülemek için kullanılır. Döngüler, `{% for ... in ... %}` yapısı ile tanımlanır ve `endfor` ile sonlandırılır.

Örnek bir şablon değişkeni ve döngüsü:

```
<ul>
    {% for sehir in sehirler %}   
        <li>{{ sehir }}</li>   
    {% endfor %}
</ul>
```

Yukarıdaki örnekte, `sehirler` adlı bir liste döngüsü ile dolaşılır ve her öğe için bir liste öğesi görüntülenir.

Django şablonları, web uygulamanızın kullanıcı arayüzünü dinamikleştirmek ve verileri görüntülemek için güçlü bir araçtır. Şablonlar, veritabanından gelen verileri veya kullanıcı girişi gibi dinamik bilgileri HTML belgesine entegre etmek için kullanılır.

Django'da HTML şablonları, web sayfalarını oluşturmanızı ve dinamik içerikleri sunmanızı sağlayan önemli bir özelliktir. Şablonlar, HTML belgelerine eklenen özel etiketler ve dil yapıları kullanılarak oluşturulur. İşte Django şablonları ve HTML kullanımı hakkında temel bilgiler:

**1\. Django Şablonları ve HTML Kullanımı:**

Django şablonları, HTML belgelerinin içine eklenen özel etiketler ve ifadeler ile oluşturulur. Bu özel etiketler ve ifadeler, dinamik verileri veya döngüler gibi Django uygulamanızın işlevselliğini temsil eder.

*   `{% %}`: Bu etiketler, kontrol yapıları ve şablon blokları için kullanılır. Örneğin, `{% if kullanici_girisli %} ... {% endif %}` ile bir koşul ifadesi tanımlanabilir.
    
*   `{{ }}`: Bu etiketler, şablon değişkenlerini içerir. Değişkenler, şablon ile iletişim kurmanızı sağlar. Örneğin, `Merhaba, {{ kullanici_isim }}` ile bir değişken içeriği görüntülenir.
    
*   `{# #}`: Bu etiketler, açıklamalar için kullanılır ve şablonda belgelendirmeler eklemek için kullanışlıdır.
    

Örnek bir Django şablonu:

```
<!DOCTYPE html>
<html>
<head>
    <title>{{ sayfa_basligi }}</title>
</head>
<body>
    <h1>Merhaba, {{ kullanici_isim }}</h1>
    {% if kullanici_girisli %}
        <p>Kullanıcı giriş yapmış.</p>
    {% else %}
        <p>Kullanıcı giriş yapmamış.</p>
    {% endif %}
    <ul>
        {% for sehir in sehirler %}
            <li>{{ sehir }}</li>
        {% endfor %}
    </ul>
</body>
</html>
```

Yukarıdaki örnekte, Django şablonları içinde değişkenler (`{{ sayfa_basligi }}`, `{{ kullanici_isim }}`), koşul ifadeleri (`{% if kullanici_girisli %}`), ve döngüler (`{% for sehir in sehirler %}`) kullanılmıştır.

**2\. Şablon Değişkenleri ve Döngüler:**

Django şablonlarında değişkenler, verilerin dinamik olarak görüntülenmesini sağlar. Değişkenler, `{{ }}` etiketleri içinde tanımlanır ve görünüm fonksiyonlarından gelen verileri temsil eder.

Döngüler, listedeki veya sorgudan dönen verileri şablonda görüntülemek için kullanılır. Döngüler, `{% for ... in ... %}` yapısı ile tanımlanır ve `endfor` ile sonlandırılır.

Örnek bir şablon değişkeni ve döngüsü:

```
<ul>   
    {% for sehir in sehirler %}   
        <li>{{ sehir }}</li>   
    {% endfor %}   
</ul>
```

Yukarıdaki örnekte, `sehirler` adlı bir liste döngüsü ile dolaşılır ve her öğe için bir liste öğesi görüntülenir.

Django şablonları, web uygulamanızın kullanıcı arayüzünü dinamikleştirmek ve verileri görüntülemek için güçlü bir araçtır. Şablonlar, veritabanından gelen verileri veya kullanıcı girişi gibi dinamik bilgileri HTML belgesine entegre etmek için kullanılır.Django'da HTML şablonları, web sayfalarını oluşturmanızı ve dinamik içerikleri sunmanızı sağlayan önemli bir özelliktir. Şablonlar, HTML belgelerine eklenen özel etiketler ve dil yapıları kullanılarak oluşturulur. İşte Django şablonları ve HTML kullanımı hakkında temel bilgiler:

**1\. Django Şablonları ve HTML Kullanımı:**

Django şablonları, HTML belgelerinin içine eklenen özel etiketler ve ifadeler ile oluşturulur. Bu özel etiketler ve ifadeler, dinamik verileri veya döngüler gibi Django uygulamanızın işlevselliğini temsil eder.

*   `{% %}`: Bu etiketler, kontrol yapıları ve şablon blokları için kullanılır. Örneğin, `{% if kullanici_girisli %} ... {% endif %}` ile bir koşul ifadesi tanımlanabilir.
    
*   `{{ }}`: Bu etiketler, şablon değişkenlerini içerir. Değişkenler, şablon ile iletişim kurmanızı sağlar. Örneğin, `Merhaba, {{ kullanici_isim }}` ile bir değişken içeriği görüntülenir.
    
*   `{# #}`: Bu etiketler, açıklamalar için kullanılır ve şablonda belgelendirmeler eklemek için kullanışlıdır.
    

Örnek bir Django şablonu:

```
<!DOCTYPE html>
<html>
<head>
    <title>{{ sayfa_basligi }}</title>
</head>
<body>
    <h1>Merhaba, {{ kullanici_isim }}</h1>

    {% if kullanici_girisli %}
        <p>Kullanıcı giriş yapmış.</p>
    {% else %}
        <p>Kullanıcı giriş yapmamış.</p>
    {% endif %}

    <ul>
        {% for sehir in sehirler %}
            <li>{{ sehir }}</li>
        {% endfor %}
    </ul>
</body>
</html>

```

Yukarıdaki örnekte, Django şablonları içinde değişkenler (`{{ sayfa_basligi }}`, `{{ kullanici_isim }}`), koşul ifadeleri (`{% if kullanici_girisli %}`), ve döngüler (`{% for sehir in sehirler %}`) kullanılmıştır.

**2\. Şablon Değişkenleri ve Döngüler:**

Django şablonlarında değişkenler, verilerin dinamik olarak görüntülenmesini sağlar. Değişkenler, `{{ }}` etiketleri içinde tanımlanır ve görünüm fonksiyonlarından gelen verileri temsil eder.

Döngüler, listedeki veya sorgudan dönen verileri şablonda görüntülemek için kullanılır. Döngüler, `{% for ... in ... %}` yapısı ile tanımlanır ve `endfor` ile sonlandırılır.

Örnek bir şablon değişkeni ve döngüsü:

```
<ul>
    {% for sehir in sehirler %}
        <li>{{ sehir }}</li>
    {% endfor %}
</ul>
```

Yukarıdaki örnekte, `sehirler` adlı bir liste döngüsü ile dolaşılır ve her öğe için bir liste öğesi görüntülenir.

Django şablonları, web uygulamanızın kullanıcı arayüzünü dinamikleştirmek ve verileri görüntülemek için güçlü bir araçtır. Şablonlar, veritabanından gelen verileri veya kullanıcı girişi gibi dinamik bilgileri HTML belgesine entegre etmek için kullanılır.Django'da HTML şablonları, web sayfalarını oluşturmanızı ve dinamik içerikleri sunmanızı sağlayan önemli bir özelliktir. Şablonlar, HTML belgelerine eklenen özel etiketler ve dil yapıları kullanılarak oluşturulur. İşte Django şablonları ve HTML kullanımı hakkında temel bilgiler:

**1\. Django Şablonları ve HTML Kullanımı:**

Django şablonları, HTML belgelerinin içine eklenen özel etiketler ve ifadeler ile oluşturulur. Bu özel etiketler ve ifadeler, dinamik verileri veya döngüler gibi Django uygulamanızın işlevselliğini temsil eder.

*   `{% %}`: Bu etiketler, kontrol yapıları ve şablon blokları için kullanılır. Örneğin, `{% if kullanici_girisli %} ... {% endif %}` ile bir koşul ifadesi tanımlanabilir.
    
*   `{{ }}`: Bu etiketler, şablon değişkenlerini içerir. Değişkenler, şablon ile iletişim kurmanızı sağlar. Örneğin, `Merhaba, {{ kullanici_isim }}` ile bir değişken içeriği görüntülenir.
    
*   `{# #}`: Bu etiketler, açıklamalar için kullanılır ve şablonda belgelendirmeler eklemek için kullanışlıdır.
    

Örnek bir Django şablonu:

```
<!DOCTYPE html>
<html>
<head>
    <title>{{ sayfa_basligi }}</title>
</head>
<body>
    <h1>Merhaba, {{ kullanici_isim }}</h1>
    
    {% if kullanici_girisli %}
        <p>Kullanıcı giriş yapmış.</p>
    {% else %}
        <p>Kullanıcı giriş yapmamış.</p>
    {% endif %}
    
    <ul>
        {% for sehir in sehirler %}
            <li>{{ sehir }}</li>
        {% endfor %}
    </ul>
</body>
</html>

```

Yukarıdaki örnekte, Django şablonları içinde değişkenler (`{{ sayfa_basligi }}`, `{{ kullanici_isim }}`), koşul ifadeleri (`{% if kullanici_girisli %}`), ve döngüler (`{% for sehir in sehirler %}`) kullanılmıştır.

**2\. Şablon Değişkenleri ve Döngüler:**

Django şablonlarında değişkenler, verilerin dinamik olarak görüntülenmesini sağlar. Değişkenler, `{{ }}` etiketleri içinde tanımlanır ve görünüm fonksiyonlarından gelen verileri temsil eder.

Döngüler, listedeki veya sorgudan dönen verileri şablonda görüntülemek için kullanılır. Döngüler, `{% for ... in ... %}` yapısı ile tanımlanır ve `endfor` ile sonlandırılır.

Örnek bir şablon değişkeni ve döngüsü:

```
<ul>   
    {% for sehir in sehirler %}   
        <li>{{ sehir }}</li>   
    {% endfor %}   
</ul>
```

Yukarıdaki örnekte, `sehirler` adlı bir liste döngüsü ile dolaşılır ve her öğe için bir liste öğesi görüntülenir.

Django şablonları, web uygulamanızın kullanıcı arayüzünü dinamikleştirmek ve verileri görüntülemek için güçlü bir araçtır. Şablonlar, veritabanından gelen verileri veya kullanıcı girişi gibi dinamik bilgileri HTML belgesine entegre etmek için kullanılır.

13\. Admin Paneli
-----------------

\- Django admin panelini özelleştirme ve kullanma

\- Veritabanı yönetimi

Django admin paneli, veritabanı yönetimi ve web uygulamanızın yönetimi için güçlü bir araçtır. Admin paneli, veritabanınıza veri eklemek, düzenlemek, silmek ve sorgulamak için kullanabileceğiniz kullanıcı dostu bir arayüze sahiptir. İşte Django admin panelini özelleştirme ve kullanma hakkında temel bilgiler:

**Django Admin Panelini Kullanma:**

Django admin paneline erişmek için önce bir süper kullanıcı hesabı oluşturmanız gerekmektedir. Süper kullanıcı hesabı oluşturmak için aşağıdaki komutu kullanabilirsiniz

`python manage.py createsuperuser `

Bu komut çalıştırıldığında, kullanıcı adı, e-posta adresi ve şifre gibi bilgileri girmeniz istenecektir. Süper kullanıcı hesabı oluşturulduktan sonra, admin paneline erişmek için `/admin/` yolunu kullanabilirsiniz. Kullanıcı adı ve şifre ile giriş yapabilirsiniz.

Django admin panelini kullanarak şunları yapabilirsiniz:

*   Veritabanına yeni veri eklemek.
    
*   Mevcut verileri düzenlemek ve güncellemek.
    
*   Verileri silmek.
    
*   Verileri sorgulamak ve filtrelemek.
    
*   İlişkisel tablolar arasındaki verileri düzenlemek.
    
*   Gruplama ve yetkilendirme ayarları yapmak.
    

**Django Admin Panelini Özelleştirme:**

Django admin panelini özelleştirmek için aşağıdaki yöntemleri kullanabilirsiniz:

1.  **admin.py Dosyası ile Veritabanı Modellerini Kaydetme:** `admin.py` dosyası içinde veritabanı modellerini kaydederek, admin panelinde bu modellerin görüntülenme şeklini ve düzenini özelleştirebilirsiniz. Örneğin, veritabanı modellerinizi kaydettikten sonra, ilgili alanları listelemeyi, filtrelemeyi veya sıralamayı ayarlayabilirsiniz.
    
2.  **Admin Site Ayarlarını Değiştirme:** `admin.py` dosyasında `admin.site.site_header`, `admin.site.site_title`, ve `admin.site.index_title` gibi ayarları kullanarak admin panelinin başlıklarını ve görünümünü özelleştirebilirsiniz.
    

Örnek `admin.py` dosyası özelleştirmeleri:

```
from django.contrib import admin
from .models import MyModel

class MyModelAdmin(admin.ModelAdmin):
    list_display = ('field1', 'field2', 'field3')
    list_filter = ('field1', 'field2')
    search_fields = ('field1', 'field2')  # Buraya uygun alanları ekleyin

admin.site.register(MyModel, MyModelAdmin)
admin.site.site_header = 'Özel Admin Paneli Başlığı'
admin.site.site_title = 'Admin Paneli'
admin.site.index_title = 'Ana Sayfa'
fa'

````

Bu özelleştirmeler, admin panelinin görünümünü ve işlevselliğini projenize göre ayarlamanıza olanak tanır.

Django admin paneli, projenizin veritabanı yönetimi ve içerik oluşturma için kullanışlı bir araçtır. Özelleştirme seçenekleri sayesinde, paneli projenizin gereksinimlerine göre uyarlayabilirsiniz.

14\. Projeyi Çalıştırma
-----------------------

\- Django geliştirme sunucusunu başlatma: \`python manage.py runserver\`

### 15\. Kaynaklar

\- [Kaynak linki](https://www.djangoproject.com/start/ "https://www.djangoproject.com/start/")

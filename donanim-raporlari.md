# Bilgisayar Mimarisi (CPU, RAM, Cache)

Bu başlık altında, bilgisayarın beyninden belleğine kadar nasıl çalıştığını anlamaya çalışacağım. Kod yazarken aslında bu parçaların nasıl işlediğini bilmek bana büyük avantaj sağlayacak.

## CPU İç Yapısı

CPU, yani işlemci, bilgisayarın “beynidir”. Kendi içinde iki temel parçaya ayrılıyor:

### ALU (Arithmetic Logic Unit)
Burası benim hesap makinem gibi. Tüm matematiksel ve mantıksal işlemleri burada yapıyorum:
- Toplama, çıkarma, çarpma, bölme  
- Karşılaştırmalar, mantıksal kontroller

### Kontrol Birimi (Control Unit)
Burası komutan gibi. ALU’ya ne yapacağını söylüyor ve CPU’nun diğer parçalarıyla veri akışını sağlıyor. Programdaki komutları tek tek okuyor ve yönlendiriyor.

---

## Cache Katmanları (L1–L2–L3)

Cache, CPU ile RAM arasındaki hızlı hafıza. Bazen RAM çok yavaş geliyor, işte cache devreye giriyor:

- **L1 Cache:** CPU’ya en yakın ve çok hızlı. Küçük ama kritik.  
- **L2 Cache:** L1’den biraz daha büyük ve biraz daha yavaş.  
- **L3 Cache:** Tüm çekirdekler arasında paylaşılıyor, büyük ama L1 kadar hızlı değil.

**Neden önemli?**  
CPU sürekli RAM’e gitseydi çok yavaş olurduk. Cache sayesinde sık kullandığım veriler çok hızlı geliyor ve işlerim hızlanıyor.

---

## RAM (Random Access Memory) Nasıl Çalışır?

RAM, bilgisayarımın geçici hafızası. Çalışan programlar ve veriler burada duruyor. Enerji kesilirse kayboluyor, yani kalıcı değil.  

- DRAM: Sürekli yenilenmesi gerekiyor  
- SRAM: Daha hızlı, genellikle cache’de kullanılıyor

CPU ile RAM arasındaki veri akışı çok önemli. Kod yazarken buradaki gecikmeleri bilmek bana optimizasyon yapma fırsatı veriyor.

---

## Kazanç

Bu konuyu anlamak bana şunları kazandırıyor:  
- Kodumun donanım seviyesinde nasıl işlediğini görebiliyorum  
- Performans odaklı daha bilinçli yazabiliyorum  
- CPU, RAM ve Cache’in nasıl etkileştiğini bilmek, bana gelecekteki projelerde büyük avantaj sağlar.
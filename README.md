# Tekstil Üretiminde Ekip Verimliliği

Üretim bilgilerini kullanarak ekiplerin gerçekleşen verimliliğini tahmin eder.

## Nasıl çalıştırılır?

Proje Python 3.12 ile test edilmiştir.

Python ile proje klasöründe powershell'de şu komutları çalıştır:

```powershell
python -m venv venv
.\venv\Scripts\Activate.ps1
pip install -r requirements.txt
```

VS Code’da notebook’lar için `venv` ortamını seçtikten sonra ve hücreleri şu sırayla çalıştırın:

1. `data_preparation.ipynb` ./data/raw klasör yolundaki CSV’yi işler ve hazır veriyi `data/processed/` klasörüne kaydeder.
2. `model_configuration.ipynb` modeli eğitir, sonuçları gösterir ve eğitilmiş modeli `models/pm25_model.joblib` olarak kaydeder.

# Application for azure
## Deployment
  1. Upewnij sie ze masz zainstalowane azure-cli
  2. Zaloguj sie:
  ```
  az login
  ```
  3. Wdrazamy projekt:
  ```
  mvn azure-functions:deploy
  ```
  4. Skopiuj pelny adres URL widoczny w danych wyjsciowych polecenia:
  ```
  Na przyklad:
  HttpExample : https://appforazure-functions-20220205004735441.azurewebsites.net/api/httpexample
  ```
  5. Dodajac " ?name=<Twoje_Imie> " na koncu wyswietlisz powitanie
  6. Do sprawdzenia logow mozesz uzyc komendy:
  ```
  func azure functionapp logstream <APP_NAME>
  ```
  **7. Pamietaj o usunieciu zasobu!:**
  ```
  az group delete --name java-functions-group
  ```

1. Установлен и настроен ADB.
2. Подключён смартфон Redmi Note 9s:
   -  adb -d tcpip 5555
   - adb connect 192.168.31.174

3. Получен скриншот экрана. 
   Команда  **adb exec-out screencap -p > screenshot.png**  позволяет сразу сохранить файл на пк без использования двух команд **adb shell screencap** и **adb pull**.
   ![](https://user-images.githubusercontent.com/81773062/118356190-bad49c00-b57c-11eb-9ed9-8852fd82a203.png)
4. С помощью команд **adb shell screenrecord /sdcard/video.mp4** и **adb pull** произведена запись экрана смартфона и файл video.mp4 получен на пк.
   ![](https://user-images.githubusercontent.com/81773062/118356202-bf995000-b57c-11eb-9d3a-101fc0e06982.gif)
5. С помощью команды **adb logcat | find "todolist" > todolist.log** отфильтрованы логи установленного ранее приложения To Do List и записаны в файл todolist.log на пк.
   ![](https://user-images.githubusercontent.com/81773062/118356192-bc9e5f80-b57c-11eb-998e-e3a7ec8aed77.png)
6. Команда **adb logcat | find "todolist"** выводит логи приложения To Do List в консоль.
   ![](https://user-images.githubusercontent.com/81773062/118356200-bdcf8c80-b57c-11eb-8f54-0ed09b7c606b.png)


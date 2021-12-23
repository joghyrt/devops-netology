# README #

1. Будет игнорироваться папка .тераформ и все ее содержимое. Папка .терраформ может лежать на любой глубине

    1.1 ***/.terraform/*

2. Будут игнорироваться файлы с расширением tfstate или содержашие в названии .tfstate.

    2.1 *.tfstate

    2.2.**.tfstate. **

3. Будут игнорироваться файлы с именем crash.log

    3.1 crash.log

4. Будут игнорироваться все файлы с расшерением tfvars

    4.1 *.tfvars

5. Будут игнорироваться файлы override.tf, override.tf.json и файлы содержащие в имени _override с расшерением .tf и _override.tf с расширением json

    5.1 override.tf, override.tf.json, *_override.tf, *_override.tf.json

6. Тут можно добавить файлы которые не должны игнорироватсья. Например !example_override.tf должен все равно показывться в unstaged если даже мы напишем в игнор *_override.tf

   6.1!example_override.tf
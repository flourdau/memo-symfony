# memo-symfony
*Mémo pour le framework php Symfony*
___


##   LINK STMFONY:
- [Symfony](https://symfony.com)
- [Symfony Documentations](https://symfony.com/doc/current/index.html)
- [Symfony Book](https://symfony.com/doc/current/the-fast-track/fr/index.html)


##   SYMFONY-CLI:
    wget https://get.symfony.com/cli/installer -O - | bash
    sudo mv /home/senacra/.symfony/bin/symfony /usr/local/bin/symfony


##   REQUIREMENTS :
    symfony check:requirements
    symfony book:check-requirements
    php bin/console about


##   INSTALL:
    symfony new my_project_name
    symfony new my_project_name --webapp
    symfony new my_project_name --fulls
    symfony new my_project_name --version=lts
    symfony new my_project_name --version=6
    symfony new my_project_name --demo
    symfony new --version=5.0-5 --book guestbook


##   DATABASES :
### Si MYSQL
    DATABASE_URL=mysql://NICKNAME:PASSWORD@127.0.0.1:3306/DB_NAME?serverVersion=5.7

### Si Mariadb
    DATABASE_URL=mysql://NICKNAME:PASSWORD@127.0.0.1:3306/DB_NAME 


##   CONSOLE :
    symfony console list make
    symfony server:ca:install
    symfony var:export
    symfony serve -d
    symfony serve:stop
    symfony console security:encode-password
    symfony php bin/phpunit
    symfony console debug:autowiring encoder
    symfony console make:docker:database
    symfony console cache:clear
    php bin/console cache:clear


##   DOCTRINE :
    symfony console make:migration
    symfony console doctrine:migrations:migrate
    symfony console doctrine:migrations:migrate -n
    symfony console doctrine:database:drop --force
    symfony console doctrine:database:create
    symfony console doctrine:schema:create


##   MAKE :
    symfony console make:entity Conference
    symfony console make:form CommentFormType Comment
    symfony console make:user Admin
    symfony console make:auth
    symfony console make:unit-test SpamCheckerTest
    symfony console make:command app:step:info
    symfony console make:controller HomeController


##   DEPENDENCES DEV :
    symfony composer req profiler --dev
    symfony composer req debug --dev
    symfony composer req maker --dev
    symfony composer req phpunit --dev
    symfony composer req browser-kit --dev
    symfony composer req orm-fixtures --dev
    symfony composer req "dama/doctrine-test-bundle:^6" --dev
    symfony composer req panther --dev


##   DEPENDENCES :
    symfony composer req logger
    symfony composer req annotations
    symfony composer req "orm:^2"
    symfony composer req "admin:^2"src/SpamChecker.php
    symfony composer req "twig:^3"
    symfony composer req "twig/intl-extra:^3"
    symfony composer req string
    symfony composer req mime
    symfony composer req security
    symfony composer req http-client
    symfony console doctrine:fixtures:load
    symfony composer req workflow
    symfony composer req mailer
    symfony composer req "twig/cssinliner-extra:^3" "twig/inky-extra:^3"
    symfony composer req process
    symfony composer req cache
    symfony composer req encore
    symfony composer req "imagine/imagine:^1.2"
    symfony console app:comment:cleanup
    symfony composer req notifier
    symfony composer req slack-notifier
    symfony composer req api
    symfony composer req twig/string-extra


##   PANEL_ADMIN:
    symfony composer req "admin:^4"  
    symfony console make:admin:dashboard
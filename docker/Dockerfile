FROM wordpress:4.9-php5.6-apache

WORKDIR /usr/src/wordpress

RUN curl -O https://raw.githubusercontent.com/wp-cli/builds/gh-pages/phar/wp-cli.phar

CMD chmod +x ./wp-cli.phar
CMD mv ./wp-cli.phar /usr/local/bin/wp

CMD wp plugin install woocommerce --activate --allow-root
CMD wp plugin install woocommerce-extra-checkout-fields-for-brazil --activate --allow-root

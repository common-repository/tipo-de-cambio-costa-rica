=== Tipo de Cambio Costa Rica ===
Contributors: arielcr
Tags: colones, dolares, tipo de cambio, costa rica
Donate link: http://arielorozco.com
Requires at least: 3.0.1
Tested up to: 4.7
Stable tag: 1.0
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Gets the exchange rate from Costa Rica's Central Bank (BCCR).

== Description ==
This plugin gets the current exchange rate from Costa Rica's Central Bank (BCCR). It allows you to insert it into any template
or with tags on any post or page. It is also possible to convert an amount of colones to dollars and vice versa through
functions in the template or also with tags in the posts.

This plugin relies on a 3rd party as a service. It uses BCCR's web service to get the exchanges rates. Service description can
be found [here](http://indicadoreseconomicos.bccr.fi.cr/indicadoreseconomicos/WebServices/wsindicadoreseconomicos.asmx)

== Installation ==
To install the plugin you must do the following:

1. Upload the plugin files to the `/wp-content/plugins/wp-tipo-cambio-cr` directory, or install the plugin through the WordPress plugins screen directly.
2. Activate the plugin through the 'Plugins' screen in WordPress

### To use the plugin on a template file

**To get the exchange rate:**

    <?php echo wptcr_tipo_cambio('COMPRA'); ?>
    <?php echo wptcr_tipo_cambio('VENTA'); ?>

**To convert a value:**

    <?php echo wptcr_convertir_colones_dolares(25000); ?>
    <?php echo wptcr_convertir_dolares_colones(100); ?>

### To use the plugin in a post or page

**Sell Exchange Rate:** `[WPTCR_TIPO_CAMBIO_COMPRA]`

**Buy Exchange Rate:** `[WPTCR_TIPO_CAMBIO_VENTA]`

**Colones to Dollars:** `[WPTCR_CONVERTIR_COLONES_DOLARES monto=20000]`

**Dollars to Colones:** `[WPTCR_CONVERTIR_DOLARES_COLONES monto=200]`

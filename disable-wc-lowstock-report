<?php

/**
 * Plugin Name:  Tijdelijk door xel: Fix woocommerce admin analytics performance issue
 * Plugin URI:
 * Description:  
 * Version:      1.0.0
 * Author:
 * Author URI:
 * License:      MIT
 */

add_filter('posts_where', function ($where, WP_Query $wp_query) {
    if ($wp_query->get('low_in_stock')) {
        $wp_query->set('low_in_stock', false);
    }

    return $where;
}, 9999, 3);

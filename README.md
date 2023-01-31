# Woocommerce shop page product display randomly
## Location
```
// Shop page product rendomly chnage
function random_shop_products() {
    $args = array(
        'post_type' => 'product',
        'posts_per_page' => 12,
        'orderby' => 'rand',
    );
    query_posts( $args );
}
add_action( 'woocommerce_before_shop_loop', 'random_shop_products' );
```


laravel 8 route problem
use App\Http\Controllers\PostController;
Route::get('/post', [PostController::class, 'index']);



-------------------- start prooduct databse use----------------
laravel 8 database show

Controller
use App\Models\Product;

public function products(){
        $products = Product::orderBy('id','desc')->get();
        return view('pages.product.index')->with('products', $products);
    }
    
@foreach($products as $product)
                        
                    @endforeach
                    
                    
-------------------- end prooduct databse use----------------

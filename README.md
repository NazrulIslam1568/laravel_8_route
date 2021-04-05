use App\Http\Controllers\PostController;
Route::get('/post', [PostController::class, 'index']);

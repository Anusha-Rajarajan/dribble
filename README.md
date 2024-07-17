# dribble
## AIM:
To Create a simplified clone of Dribble.
## Program:
~~~
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Design Gallery</title>
  <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css">
  <style>
    body {
      background-color: #f5f5f5;
    }
    .navbar {
      background-color: #333;
    }
    .navbar-brand, .navbar-nav .nav-link {
      color: #fff;
    }
    .navbar-brand:hover, .navbar-nav .nav-link:hover {
      color: #ddd;
    }
    .btn-pink {
      background-color: #ff4081;
      color: #fff;
    }
    .gallery-header {
      margin-top: 5px;
      margin-bottom: 5px;
      text-align: center;
    }
    .gallery-header h1 {
      display: inline-block;
    }
    .gallery-header .btn {
      float: right;
    }
    .card {
      margin-bottom: 10px;
      border: none;
      border-radius: 10px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
    }
    .card-body {
      padding: 1rem;
    }
    .card-title {
      font-size: 1.1rem;
      margin-bottom: 0.1rem;
    }
    .card-footer {
      background-color: transparent;
      border-top: none;
      padding-top: 0;
    }
    .card-footer .author-info {
      display: flex;
      align-items: center;
    }
    .card-footer img {
      width: 30px;
      height: 30px;
      border-radius: 50%;
      margin-right: 10px;
    }
    .card-footer .author-name {
      font-weight: bold;
      margin-right: 2px;
    }
    .card-footer .author-status {
      color: #777;
      font-size: 0.9rem;
    }
    .card-footer .stats {
      margin-left: auto;
      display: flex;
      align-items: center;
    }
    .card-footer .stats .stat-item {
      margin-left: 10px;
      font-size: 0.9rem;
      color: #777;
    }
    .card-footer .stats .stat-item i {
      margin-right: 2px;
    }
    .dropdown .dropdown-toggle {
      color: #000;
    }
    .dropdowns {
      display: flex;
      justify-content: center;
      margin-bottom: 10px;
    }
    .dropdowns .dropdown {
      margin: 0 1px;
    }
  </style>
</head>
<body>
  <nav class="navbar navbar-expand-lg">
    <a class="navbar-brand" href="#">Dribbble</a>
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNav">
      <ul class="navbar-nav ml-auto">
        <li class="nav-item">
          <a class="nav-link" href="#">Shots</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Designers</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Teams</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Community</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Jobs</a>
        </li>
      </ul>
    </div>
  </nav>

  <div class="container">
    <div class="gallery-header">
      <h1>What are you working on? Dribbble is show and tell for designers.</h1>
      <button class="btn btn-pink">Learn more</button>
      <button class="btn btn-primary">Sign up</button>
    </div>
    <div class="dropdowns">
      <div class="dropdown">
        <button class="btn dropdown-toggle" type="button" id="dropdownMenuButton" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
          Popular
        </button>
        <div class="dropdown-menu" aria-labelledby="dropdownMenuButton">
          <a class="dropdown-item" href="#">Popular</a>
          <a class="dropdown-item" href="#">Newest</a>
        </div>
      </div>
      <div class="dropdown">
        <button class="btn dropdown-toggle" type="button" id="dropdownMenuButton2" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
          Shots
        </button>
        <div class="dropdown-menu" aria-labelledby="dropdownMenuButton2">
          <a class="dropdown-item" href="#">Shots</a>
          <a class="dropdown-item" href="#">Projects</a>
        </div>
      </div>
      <div class="dropdown">
        <button class="btn dropdown-toggle" type="button" id="dropdownMenuButton3" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
          Now
        </button>
        <div class="dropdown-menu" aria-labelledby="dropdownMenuButton3">
          <a class="dropdown-item" href="#">Now</a>
          <a class="dropdown-item" href="#">Week</a>
          <a class="dropdown-item" href="#">Month</a>
        </div>
      </div>
    </div>

    <div class="row">
        
      <div class="col-md-3 col-sm-6">
        <div class="card">
          <img src="image1.jpg" class="card-img-top" alt="Design Preview">
          <div class="card-body">
            <h5 class="card-title">Plainthing Studio</h5>
            <div class="card-text">
              <button class="btn btn-light"><i class="far fa-bookmark"></i></button>
              <button class="btn btn-light"><i class="far fa-heart"></i></button>
            </div>
          </div>
          <div class="card-footer">
            <div class="author-info">
              <img src="a1.png" alt="Author">
              <div>
                <div class="author-status">PRO</div>
              </div>
            </div>
            <div class="stats">
              <div class="stat-item"><i class="fas fa-heart"></i> 122</div>
              <div class="stat-item"><i class="fas fa-eye"></i> 29.8k</div>
            </div>
          </div>
        </div>
      </div>

      <div class="col-md-3 col-sm-6">
        <div class="card">
          <img src="image2.png" class="card-img-top" alt="Design Preview">
          <div class="card-body">
            <h5 class="card-title">Vedant Hedge</h5>
            <div class="card-text">
              <button class="btn btn-light"><i class="far fa-bookmark"></i></button>
              <button class="btn btn-light"><i class="far fa-heart"></i></button>
            </div>
          </div>
          <div class="card-footer">
            <div class="author-info">
              <img src="a2.png" alt="Author">
              <div>
                <div class="author-status">PRO</div>
              </div>
            </div>
            <div class="stats">
              <div class="stat-item"><i class="fas fa-heart"></i> 150</div>
              <div class="stat-item"><i class="fas fa-eye"></i> 10.5k</div>
            </div>
          </div>
        </div>
      </div>

      <div class="col-md-3 col-sm-6">
        <div class="card">
          <img src="image3.jpg" class="card-img-top" alt="Design Preview">
          <div class="card-body">
            <h5 class="card-title">One week wonders</h5>
            <div class="card-text">
              <button class="btn btn-light"><i class="far fa-bookmark"></i></button>
              <button class="btn btn-light"><i class="far fa-heart"></i></button>
            </div>
          </div>
          <div class="card-footer">
            <div class="author-info">
              <img src="a3.jpg" alt="Author">
              <div>
                <div class="author-status">PRO</div>
              </div>
            </div>
            <div class="stats">
              <div class="stat-item"><i class="fas fa-heart"></i> 150</div>
              <div class="stat-item"><i class="fas fa-eye"></i> 10.5k</div>
            </div>
          </div>
        </div>
      </div>

      <div class="col-md-3 col-sm-6">
        <div class="card">
          <img src="image4.jpg" class="card-img-top" alt="Design Preview">
          <div class="card-body">
            <h5 class="card-title">Emotion Tracker</h5>
            <div class="card-text">
              <button class="btn btn-light"><i class="far fa-bookmark"></i></button>
              <button class="btn btn-light"><i class="far fa-heart"></i></button>
            </div>
          </div>
          <div class="card-footer">
            <div class="author-info">
              <img src="a4.png" alt="Author">
              <div>
                <div class="author-status">PRO</div>
              </div>
            </div>
            <div class="stats">
              <div class="stat-item"><i class="fas fa-heart"></i> 150</div>
              <div class="stat-item"><i class="fas fa-eye"></i> 10.5k</div>
            </div>
          </div>
        </div>
      </div>

      <div class="col-md-3 col-sm-6">
        <div class="card">
          <img src="image5.jpg" class="card-img-top" alt="Design Preview">
          <div class="card-body">
            <h5 class="card-title">Fire Fighters</h5>
            <div class="card-text">
              <button class="btn btn-light"><i class="far fa-bookmark"></i></button>
              <button class="btn btn-light"><i class="far fa-heart"></i></button>
            </div>
          </div>
          <div class="card-footer">
            <div class="author-info">
              <img src="a1.png" alt="Author">
              <div>
                <div class="author-status">PRO</div>
              </div>
            </div>
            <div class="stats">
              <div class="stat-item"><i class="fas fa-heart"></i> 150</div>
              <div class="stat-item"><i class="fas fa-eye"></i> 10.5k</div>
            </div>
          </div>
        </div>
      </div>

      <div class="col-md-3 col-sm-6">
        <div class="card">
          <img src="image6.jpg" class="card-img-top" alt="Design Preview">
          <div class="card-body">
            <h5 class="card-title">Fire or DumsterFire</h5>
            <div class="card-text">
              <button class="btn btn-light"><i class="far fa-bookmark"></i></button>
              <button class="btn btn-light"><i class="far fa-heart"></i></button>
            </div>
          </div>
          <div class="card-footer">
            <div class="author-info">
              <img src="a2.png" alt="Author">
              <div>
                <div class="author-status">PRO</div>
              </div>
            </div>
            <div class="stats">
              <div class="stat-item"><i class="fas fa-heart"></i> 150</div>
              <div class="stat-item"><i class="fas fa-eye"></i> 10.5k</div>
            </div>
          </div>
        </div>
      </div>

      <div class="col-md-3 col-sm-6">
        <div class="card">
          <img src="image7.png" class="card-img-top" alt="Design Preview">
          <div class="card-body">
            <h5 class="card-title">Howdy</h5>
            <div class="card-text">
              <button class="btn btn-light"><i class="far fa-bookmark"></i></button>
              <button class="btn btn-light"><i class="far fa-heart"></i></button>
            </div>
          </div>
          <div class="card-footer">
            <div class="author-info">
              <img src="a3.jpg" alt="Author">
              <div>
                <div class="author-status">PRO</div>
              </div>
            </div>
            <div class="stats">
              <div class="stat-item"><i class="fas fa-heart"></i> 150</div>
              <div class="stat-item"><i class="fas fa-eye"></i> 10.5k</div>
            </div>
          </div>
        </div>
      </div>

      <div class="col-md-3 col-sm-5">
        <div class="card">
          <img src="image8.jpg" class="card-img-top" alt="Design Preview">
          <div class="card-body">
            <h5 class="card-title">Hermit Hermes</h5>
            <div class="card-text">
              <button class="btn btn-light"><i class="far fa-bookmark"></i></button>
              <button class="btn btn-light"><i class="far fa-heart"></i></button>
            </div>
          </div>
          <div class="card-footer">
            <div class="author-info">
              <img src="a4.png" alt="Author">
              <div>
                <div class="author-status">PRO</div>
              </div>
            </div>
            <div class="stats">
              <div class="stat-item"><i class="fas fa-heart"></i> 150</div>
              <div class="stat-item"><i class="fas fa-eye"></i> 10.5k</div>
            </div>
          </div>
        </div>
      </div>

      <div class="col-md-3 col-sm-6">
      <div class="card">
        <img src="image9.png" class="card-img-top" alt="Design Preview">
        <div class="card-body">
          <h5 class="card-title">Simms Fishing Apparel Design</h5>
          <div class="card-text">
            <button class="btn btn-light"><i class="far fa-bookmark"></i></button>
            <button class="btn btn-light"><i class="far fa-heart"></i></button>
          </div>
        </div>
        <div class="card-footer">
          <div class="author-info">
            <img src="a1.png" alt="Author">
            <div>
              <div class="author-status">PRO</div>
            </div>
          </div>
          <div class="stats">
            <div class="stat-item"><i class="fas fa-heart"></i> 150</div>
            <div class="stat-item"><i class="fas fa-eye"></i> 10.5k</div>
          </div>
        </div>
      </div>
    </div>
    <div class="col-md-3 col-sm-6">
      <div class="card">
        <img src="image10.jpg" class="card-img-top" alt="Design Preview">
        <div class="card-body">
          <h5 class="card-title">The Archer</h5>
          <div class="card-text">
            <button class="btn btn-light"><i class="far fa-bookmark"></i></button>
            <button class="btn btn-light"><i class="far fa-heart"></i></button>
          </div>
        </div>
        <div class="card-footer">
          <div class="author-info">
            <img src="a2.png" alt="Author">
            <div>
              <div class="author-status">PRO</div>
            </div>
          </div>
          <div class="stats">
            <div class="stat-item"><i class="fas fa-heart"></i> 150</div>
            <div class="stat-item"><i class="fas fa-eye"></i> 10.5k</div>
          </div>
        </div>
      </div>
    </div>
    <div class="col-md-3 col-sm-6">
      <div class="card">
        <img src="image11.png" class="card-img-top" alt="Design Preview">
        <div class="card-body">
          <h5 class="card-title">Coric Design</h5>
          <div class="card-text">
            <button class="btn btn-light"><i class="far fa-bookmark"></i></button>
            <button class="btn btn-light"><i class="far fa-heart"></i></button>
          </div>
        </div>
        <div class="card-footer">
          <div class="author-info">
            <img src="a4.png" alt="Author">
            <div>
              <div class="author-status">PRO</div>
            </div>
          </div>
          <div class="stats">
            <div class="stat-item"><i class="fas fa-heart"></i> 150</div>
            <div class="stat-item"><i class="fas fa-eye"></i> 10.5k</div>
          </div>
        </div>
      </div>
    </div>
    <div class="col-md-3 col-sm-6">
      <div class="card">
        <img src="image12.jpg" class="card-img-top" alt="Design Preview">
        <div class="card-body">
          <h5 class="card-title">Coric Design</h5>
          <div class="card-text">
            <button class="btn btn-light"><i class="far fa-bookmark"></i></button>
            <button class="btn btn-light"><i class="far fa-heart"></i></button>
          </div>
        </div>
        <div class="card-footer">
          <div class="author-info">
            <img src="a3.jpg" alt="Author">
            <div>
              <div class="author-status">PRO</div>
            </div>
          </div>
          <div class="stats">
            <div class="stat-item"><i class="fas fa-heart"></i> 150</div>
            <div class="stat-item"><i class="fas fa-eye"></i> 10.5k</div>
          </div>
        </div>
      </div>
    </div>
    

    </div>
  </div>

  <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
  <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.5.4/dist/umd/popper.min.js"></script>
  <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>
</body>
</html>
~~~
## Output:
![alt text](out1.png)

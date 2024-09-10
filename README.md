# SWT
<!DOCTYPE html>
<html>
    <head>
        <title>Login Banana</title>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <link rel="stylesheet" type="text/css" href="css/login.css">
        <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.0/css/bootstrap.min.css">
        <link href="https://stackpath.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css" rel="stylesheet">
    </head>
    <body>
        <div class="container">
            <div class="row px-3">
                <div class="col-lg-10 col-xl-9 card flex-row mx-auto px-0">
                    <div class="img-left d-none d-md-flex"></div>
                    
                    <div class="card-body">
                        <h1 class="title text-center mt-4">Sign In</h1>
                        <form action="MainController" method="POST" class="form-box px-3">
                            <div class="form-input">
                                <span><i class="fa fa-user"></i></span>
                                <input type="text" name="txtUserId" placeholder="UserID" tabindex="10" required/><br/>
                            </div>
                            <div class="form-input">
                                <span><i class="fa fa-key"></i></span>
                                <input type="password" name="txtPassword" placeholder="Password" required/><br/>
                            </div>
                            <div class="text-center mb-3">
                                <br>
                            </div>
                            <div class="mb-3">
                                <button type="reset" value="Reset" class="btn btn-block"/>
                                RESET
                                </button>
                            </div>
                            <div class="mb-3">
                                <button type="submit" name="action" value="Login" class="btn btn-block"/>
                                LOGIN
                                </button>
                            </div>
                            <div class="text-right">
                                <a href="#" class="forget-link">
                                Forget Password?
                                </a>
                            </div>
                            <br>
                            <div class="row mb-3" id="signup">
                                <div class="col-6">
                                    <a href="create.jsp" class="btn btn-block btn-social btn-create">
                                    Sign Up
                                    </a>
                                </div>
                            </div>
                        </form>
                    </div>
                </div>
            </div>
        </div>
    <script>
        function addLink() {
            var linkContainer = document.createElement('div');
            linkContainer.className = 'col-6';
            
            var link = document.createElement('a');
            link.href = '#';
            link.className = 'btn btn-block btn-social';
            link.textContent = 'New Link';
            
            linkContainer.appendChild(link);
            
            var signupRow = document.getElementById('signup');
            signupRow.appendChild(linkContainer);
        }

        // Call the function when the page loads
        window.onload = addLink;
    </script>
    </body>
</html>

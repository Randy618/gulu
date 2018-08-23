<template>
    <div>
        <div class="header">
            <h2><strong>Buttons</strong></h2>
            <div class="breadcrumb-wrapper">
                <ol class="breadcrumb">
                    <li>
                        <a href="#">Make</a>
                    </li>
                    <li>
                        <a href="#">Pages</a>
                    </li>
                    <li class="active">Buttons</li>
                </ol>
            </div>
        </div>
        <div class="row">
            <div class="col-lg-12 portlets">
                <div class="panel">
                    <div class="panel-header panel-controls">
                        <h3><i class="icon-layers"></i> Choose your <strong>Style</strong></h3>
                    </div>
                    <div class="panel-content">
                        <p>You can set different colors by adding <code>btn-primary</code> class for example. Want embossed button? Add <code>btn-embossed</code> class, that's it!</p>
                        <div class="row">
                            <div class="col-md-6">
                                <h3><strong>Classic</strong> Style</h3>
                                <p>Default style with <code>btn</code> class.</p>
                                <m-button type="white">White</m-button>
                                <m-button type="default">Default</m-button>
                                <m-button type="primary">Primary</m-button>
                                <m-button type="success">Success</m-button>
                                <m-button type="info">Info</m-button>
                                <m-button type="blue">Blue</m-button>
                                <m-button type="warning">Warning</m-button>
                                <m-button type="danger">Danger</m-button>
                                <m-button type="dark">Dark</m-button>
                            </div>
                            <div class="col-md-6">
                                <h3><strong>Embossed</strong> style</h3>
                                <p>How to use? Just add <code>btn-embossed</code> class.</p>
                                <m-button type="white" embossed>White</m-button>
                                <m-button type="default" embossed>Default</m-button>
                                <m-button type="primary" embossed>Primary</m-button>
                                <m-button type="success" embossed>Success</m-button>
                                <m-button type="info" embossed>Info</m-button>
                                <m-button type="warning" embossed>Warning</m-button>
                                <m-button type="danger" embossed>Danger</m-button>
                                <m-button type="dark" embossed>Dark</m-button>
                            </div>
                        </div>
                        <div class="row m-t-30">
                            <div class="col-md-6">
                                <h3><strong>Rounded</strong> style</h3>
                                <p>How to use? Just add <code>btn-rounded</code> class.</p>
                                <m-button type="default" rounded>Default</m-button>
                                <m-button type="primary" rounded>Primary</m-button>
                                <m-button type="success" rounded>Success</m-button>
                                <m-button type="info" rounded>Info</m-button>
                                <m-button type="warning" rounded>Warning</m-button>
                                <m-button type="danger" rounded>Danger</m-button>
                                <m-button type="dark" rounded>Dark</m-button>
                            </div>
                            <div class="col-md-6">
                                <h3><strong>Transparent</strong> style</h3>
                                <p>How to use? Just add <code>btn-transparent</code> class.</p>
                                <m-button type="default" transparent>Default</m-button>
                                <m-button type="primary" transparent>Primary</m-button>
                                <m-button type="success" transparent>Success</m-button>
                                <m-button type="warning" transparent>Warning</m-button>
                                <m-button type="danger" transparent>Danger</m-button>
                                <m-button type="dark" transparent>Dark</m-button>
                            </div>
                        </div>
                        <div class="row m-t-30">
                            <div class="col-md-6">
                                <h3><strong>Square</strong> style</h3>
                                <p>How to use? Just add <code>btn-square</code> class.</p>
                                <m-button type="default" square>Default</m-button>
                                <m-button type="primary" square>Primary</m-button>
                                <m-button type="success" square>Success</m-button>
                                <m-button type="info" square>Info</m-button>
                                <m-button type="warning" square>Warning</m-button>
                                <m-button type="danger" square>Danger</m-button>
                                <m-button type="dark" square>Dark</m-button>
                            </div>
                            <div class="col-md-6">
                                <h3><strong>Mixed</strong> style</h3>
                                <p>Make your style unique by mixing it! For example <code>btn-primary btn-square btn-embossed</code> class.</p>
                                <m-button type="primary" square embossed>Primary</m-button>
                                <m-button type="success" rounded>Success</m-button>
                                <m-button type="info" transparent rounded>Info</m-button>
                                <m-button type="warning" rounded embossed>Warning</m-button>
                                <m-button type="danger" transparent>Danger</m-button>
                                <m-button type="dark" square>Dark</m-button>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="col-lg-12 portlets">
                <div class="panel">
                    <div class="panel-header panel-controls">
                        <h3><i class="icon-bulb"></i> <strong>Group</strong> Buttons</h3>
                    </div>
                    <div class="panel-content">
                        <p>
                            Group buttons are great if you want to display a group of actions. To do that, just put you buttons inside a <code>btn-group</code> class div.
                        </p>
                        <div class="row">
                            <div class="col-md-4">
                                <h3><strong>Horizontal</strong> group</h3>
                                <br>
                                <m-button-group>
                                    <m-button type="primary" active icon="fa-align-left"></m-button>
                                    <m-button type="primary" icon="fa-align-justify"></m-button>
                                    <m-button type="primary" icon="fa-align-right"></m-button>
                                </m-button-group>
                                <br>
                                <br>
                                <m-button-group>
                                    <m-button type="danger" icon="fa-align-left"></m-button>
                                    <m-button type="danger">1</m-button>
                                    <m-button type="danger" active>2</m-button>
                                    <m-button type="danger">3</m-button>
                                    <m-button type="danger">4</m-button>
                                    <m-button type="danger" icon="fa-align-right"></m-button>
                                </m-button-group>

                            </div>
                            <div class="col-md-3">
                                <h3><strong>Vertical</strong> group</h3>
                                <br>
                                <m-button-group vertical>
                                    <m-button type="primary" active icon="fa-align-left"></m-button>
                                    <m-button type="primary" icon="fa-align-justify"></m-button>
                                    <m-button type="primary" icon="fa-align-right"></m-button>
                                </m-button-group>
                                <m-button-group vertical>
                                    <m-button type="primary" active icon="fa-facebook"></m-button>
                                    <m-button type="danger" icon="fa-google-plus"></m-button>
                                    <m-button type="blue" icon="fa-twitter"></m-button>
                                </m-button-group>
                                <m-button-group vertical>
                                    <m-button type="dark" active>1</m-button>
                                    <m-button type="dark">2</m-button>
                                    <m-button type="dark">3</m-button>
                                </m-button-group>
                            </div>
                            <div class="col-md-5">
                                <h3><strong>Nested</strong> button groups</h3>
                                <br>
                                <m-button-group>
                                    <m-button type="white" icon="icon-user">Profile</m-button>
                                    <m-button type="white" icon="icon-user">Profile</m-button>
                                    <m-button type="white" active icon="icon-user">Profile</m-button>
                                    <m-button-group>
                                        <m-button type="white"></m-button>
                                    </m-button-group>
                                </m-button-group>
                                <div class="btn-group">
                                    <button type="button" class="btn btn-white"><i class="icon-user"></i> Profile</button>
                                    <button type="button" class="btn btn-white"><i class="icon-envelope"></i> Messages</button>
                                    <button type="button" class="btn btn-white active"><i class="icon-settings"></i> Settings</button>
                                    <div class="btn-group">
                                        <button type="button" class="btn btn-white dropdown-toggle" data-toggle="dropdown">
                                            <i class="fa fa-ellipsis-horizontal"></i> More <i class="fa fa-angle-down"></i>
                                        </button>
                                        <ul class="dropdown-menu">
                                            <li>
                                                <a href="#">Dropdown link</a>
                                            </li>
                                            <li>
                                                <a href="#">Dropdown link</a>
                                            </li>
                                        </ul>
                                    </div>
                                </div>
                                <br>
                                <br>
                                <div class="btn-group">
                                    <button type="button" class="btn btn-primary"><i class="icon-user"></i> Profile</button>
                                    <button type="button" class="btn btn-dark"><i class="icon-envelope"></i> Messages</button>
                                    <button type="button" class="btn btn-warning active"><i class="icon-settings"></i> Settings</button>
                                    <div class="btn-group">
                                        <button type="button" class="btn btn-danger dropdown-toggle" data-toggle="dropdown">
                                            <i class="fa fa-ellipsis-horizontal"></i> More <i class="fa fa-angle-down"></i>
                                        </button>
                                        <ul class="dropdown-menu">
                                            <li>
                                                <a href="#">Dropdown link</a>
                                            </li>
                                            <li>
                                                <a href="#">Dropdown link</a>
                                            </li>
                                        </ul>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="panel">
                    <div class="panel-header">
                        <h3><i class="icon-bulb"></i> <strong>Icons</strong> Buttons</h3>
                    </div>
                    <div class="panel-content">
                        <p>You can add icons on the left or right side of button with color you want. Perfect for action buttons and social connection.</p>
                        <div class="row">
                            <div class="col-md-4">
                                <div class="row">
                                    <div class="col-md-12">
                                        <h3><strong>Icons</strong> styled button</h3>
                                        <m-button type="blue" size="sm" icon="fa-twitter"></m-button>
                                        <m-button type="primary" size="sm" icon="fa-facebook"></m-button>
                                        <m-button type="danger" size="sm" icon="fa-google-plus"></m-button>
                                        <m-button type="dark" size="sm" icon="fa-info"></m-button>
                                        <m-button type="danger" size="sm" icon="fa-heart"></m-button>
                                        <m-button type="info" size="sm" icon="fa-map-marker"></m-button>
                                    </div>
                                </div>
                                <div class="row">
                                    <div class="col-md-12">
                                        <h3><strong>Icons</strong> rounded button</h3>
                                        <m-button size="sm" iconRounded rounded icon="fa-twitter" type="info"></m-button>
                                        <m-button size="sm" iconRounded rounded icon="fa-facebook" type="primary"></m-button>
                                        <m-button size="sm" iconRounded rounded icon="fa-google-plus" type="danger"></m-button>
                                        <m-button size="sm" iconRounded rounded icon="fa-power-off" type="default"></m-button>
                                        <m-button size="sm" iconRounded rounded icon="fa-heart" type="danger"></m-button>
                                        <m-button size="sm" iconRounded rounded icon="fa-plus" type="dark"></m-button>
                                        <m-button size="sm" iconRounded rounded icon="fa-info" type="danger"></m-button>
                                    </div>
                                </div>
                            </div>
                            <div class="col-md-4">
                                <h3><strong>Icons</strong> styled button</h3>
                                <m-button type="dark" icon="icon-cloud-upload">Upload</m-button>
                                <m-button type="primary" icon="icon-like">I like</m-button>
                                <m-button type="success" icon="icons-office-51">I agree</m-button>
                                <m-button type="white" icon="fa-plus">More</m-button>
                                <m-button type="danger" icon="icon-link">Link</m-button>
                                <m-button type="info" icon="icon-bubble">Comment</m-button>
                                ----------------------------------------------------
                                <button type="button" class="btn btn-dark"><i class="icon-cloud-upload"></i> Upload</button>
                                <button type="button" class="btn btn-primary"><i class="icon-like"></i> I like</button>
                                <button type="button" class="btn btn-success"><i class="icons-office-51"></i> I agree</button>
                                <button type="button" class="btn btn-white"><i class="fa fa-plus"></i> More</button>
                                <button type="button" class="btn btn-danger"><i class="icon-link"></i> Link</button>
                                <button type="button" class="btn btn-info"><i class="icon-bubble"></i> Comment</button>
                            </div>
                            <div class="col-md-4">
                                <h3><strong>Block Social</strong> Buttons</h3>
                                <m-button type="primary" block icon="fa-facebook" size="lg" pull="left">Connect with Facebook</m-button>
                                <m-button type="blue" block icon="fa-twitter" size="lg" pull="left">Login with Twitter</m-button>
                                <m-button type="danger" block icon="fa-google-plus" size="lg" pull="left">Connect with Google</m-button>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="panel">
                    <div class="panel-header panel-controls">
                        <h3><i class="icon-bulb"></i> <strong>Loading State</strong> &amp; <strong>Size</strong> Buttons</h3>
                    </div>
                    <div class="panel-content">
                        <div class="row">
                            <div class="col-md-6">
                                <h3><strong>Loading</strong> button <small>Click to see loading state</small></h3>
                                <p>Loading state are perfect for login, register or form submission.</p>
                                <m-button type="dark" icon="fa-upload" loading="expand-left">Expand Left</m-button>
                                <m-button type="success" icon="fa-upload" loading="expand-right">Expand Right</m-button>
                                <m-button type="info" icon="fa-upload" loading="zoom-in">Zoom In</m-button>
                                <div class="row">
                                    <div class="progress-demo col-md-6">
                                        <m-button type="danger" block loading="zoom-in">Progress Bar Style</m-button>
                                    </div>
                                </div>
                            </div>
                            <div class="col-md-6">
                                <h3><strong>Size</strong> Buttons <small>for small to Huge effect</small></h3>
                                <p>You can choose your size by simply adding a class like <code>btn-sm</code> for small button.</p>
                                <m-button type="primary" size="sm">Small button</m-button>
                                <m-button type="primary">Medium button</m-button>
                                <m-button type="primary" size="lg">Big button</m-button>
                                <m-button type="primary" size="hg">Huge button</m-button>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="panel">
                    <div class="panel-header">
                        <h3><i class="icon-bulb"></i> <strong>Dropdown</strong> Buttons</h3>
                    </div>
                    <div class="panel-content">
                        <p>Use any button to trigger a dropdown menu by placing it within a <code>.btn-group</code> and providing the proper menu markup.</p>
                        <div class="row">
                            <div class="col-md-4 clearfix">
                                <h3><strong>Simple</strong> Dropdown</h3>
                                <div class="m-b-10 f-left">
                                    <div class="btn-group" dropdown>
                                        <button type="button" class="btn btn-default dropdown-toggle" data-toggle="dropdown">
                                            Default <span class="caret"></span>
                                        </button>
                                        <span class="dropdown-arrow"></span>
                                        <ul class="dropdown-menu" role="menu">
                                            <li>
                                                <a href="#">Action</a>
                                            </li>
                                            <li>
                                                <a href="#">Another action</a>
                                            </li>
                                            <li>
                                                <a href="#">Something else here</a>
                                            </li>
                                            <li class="divider"></li>
                                            <li>
                                                <a href="#">Separated link</a>
                                            </li>
                                        </ul>
                                    </div>
                                </div>
                                <div class="m-b-10 f-left">
                                    <div class="btn-group" dropdown>
                                        <button type="button" class="btn btn-primary dropdown-toggle" data-toggle="dropdown">
                                            Primary <span class="caret"></span>
                                        </button>
                                        <span class="dropdown-arrow"></span>
                                        <ul class="dropdown-menu" role="menu">
                                            <li>
                                                <a href="#">Action</a>
                                            </li>
                                            <li>
                                                <a href="#">Another action</a>
                                            </li>
                                            <li>
                                                <a href="#">Something else here</a>
                                            </li>
                                        </ul>
                                    </div>
                                </div>
                                <div class="m-b-10 f-left">
                                    <div class="btn-group" dropdown>
                                        <button type="button" dropdown-toggle class="btn btn-success dropdown-toggle" data-toggle="dropdown">
                                            Success <span class="caret"></span>
                                        </button>
                                        <span class="dropdown-arrow"></span>
                                        <ul class="dropdown-menu" role="menu">
                                            <li>
                                                <a href="#">Action</a>
                                            </li>
                                            <li>
                                                <a href="#">Another action</a>
                                            </li>
                                            <li>
                                                <a href="#">Something else here</a>
                                            </li>
                                            <li class="divider"></li>
                                            <li>
                                                <a href="#">Separated link</a>
                                            </li>
                                        </ul>
                                    </div>
                                </div>
                                <div class="m-b-10 f-left">
                                    <div class="btn-group" dropdown>
                                        <button type="button" dropdown-toggle class="btn btn-info dropdown-toggle" data-toggle="dropdown">
                                            Info <span class="caret"></span>
                                        </button>
                                        <span class="dropdown-arrow"></span>
                                        <ul class="dropdown-menu" role="menu">
                                            <li>
                                                <a href="#">Action</a>
                                            </li>
                                            <li>
                                                <a href="#">Another action</a>
                                            </li>
                                            <li>
                                                <a href="#">Something else here</a>
                                            </li>
                                            <li class="divider"></li>
                                            <li>
                                                <a href="#">Separated link</a>
                                            </li>
                                        </ul>
                                    </div>
                                </div>
                                <div class="m-b-10 f-left">
                                    <div class="btn-group" dropdown>
                                        <button type="button"  dropdown-toggle class="btn btn-warning dropdown-toggle" data-toggle="dropdown">
                                            Warning <span class="caret"></span>
                                        </button>
                                        <span class="dropdown-arrow"></span>
                                        <ul class="dropdown-menu" role="menu">
                                            <li>
                                                <a href="#">Action</a>
                                            </li>
                                            <li>
                                                <a href="#">Another action</a>
                                            </li>
                                            <li>
                                                <a href="#">Something else here</a>
                                            </li>
                                            <li class="divider"></li>
                                            <li>
                                                <a href="#">Separated link</a>
                                            </li>
                                        </ul>
                                    </div>
                                </div>
                                <div class="m-b-10 f-left">
                                    <div class="btn-group" dropdown>
                                        <button type="button" dropdown class="btn btn-danger dropdown-toggle" data-toggle="dropdown">
                                            Danger <span class="caret"></span>
                                        </button>
                                        <span class="dropdown-arrow"></span>
                                        <ul class="dropdown-menu" role="menu">
                                            <li>
                                                <a href="#">Action</a>
                                            </li>
                                            <li>
                                                <a href="#">Another action</a>
                                            </li>
                                            <li>
                                                <a href="#">Something else here</a>
                                            </li>
                                            <li class="divider"></li>
                                            <li>
                                                <a href="#">Separated link</a>
                                            </li>
                                        </ul>
                                    </div>
                                </div>
                            </div>
                            <div class="col-md-4 clearfix">
                                <h3><strong>Split</strong> Dropdown <small>for small to Huge effect</small></h3>
                                <div class="m-b-10 f-left">
                                    <div class="btn-group" dropdown>
                                        <button type="button" class="btn btn-danger">Action</button>
                                        <button type="button" dropdown-toggle class="btn btn-danger dropdown-toggle" data-toggle="dropdown">
                                            <span class="caret"></span>
                                            <span class="sr-only">Toggle Dropdown</span>
                                        </button>
                                        <span class="dropdown-arrow"></span>
                                        <ul class="dropdown-menu" role="menu">
                                            <li>
                                                <a href="#">Action</a>
                                            </li>
                                            <li>
                                                <a href="#">Another action</a>
                                            </li>
                                            <li>
                                                <a href="#">Something else here</a>
                                            </li>
                                            <li class="divider"></li>
                                            <li>
                                                <a href="#">Separated link</a>
                                            </li>
                                        </ul>
                                    </div>
                                </div>
                                <div class="m-b-10 f-left">
                                    <div class="btn-group" dropdown>
                                        <button type="button" class="btn btn-success">Action</button>
                                        <button type="button" dropdown-toggle class="btn btn-success dropdown-toggle" data-toggle="dropdown">
                                            <span class="caret"></span>
                                            <span class="sr-only">Toggle Dropdown</span>
                                        </button>
                                        <span class="dropdown-arrow"></span>
                                        <ul class="dropdown-menu" role="menu">
                                            <li>
                                                <a href="#">Action</a>
                                            </li>
                                            <li>
                                                <a href="#">Another action</a>
                                            </li>
                                            <li>
                                                <a href="#">Something else here</a>
                                            </li>
                                            <li class="divider"></li>
                                            <li>
                                                <a href="#">Separated link</a>
                                            </li>
                                        </ul>
                                    </div>
                                </div>
                                <div class="m-b-10 f-left">
                                    <div class="btn-group" dropdown>
                                        <button type="button" class="btn btn-white">Action</button>
                                        <button dropdown-toggle type="button" class="btn btn-white dropdown-toggle" data-toggle="dropdown">
                                            <span class="caret"></span>
                                            <span class="sr-only">Toggle Dropdown</span>
                                        </button>
                                        <span class="dropdown-arrow"></span>
                                        <ul class="dropdown-menu" role="menu">
                                            <li>
                                                <a href="#">Action</a>
                                            </li>
                                            <li>
                                                <a href="#">Another action</a>
                                            </li>
                                            <li>
                                                <a href="#">Something else here</a>
                                            </li>
                                            <li class="divider"></li>
                                            <li>
                                                <a href="#">Separated link</a>
                                            </li>
                                        </ul>
                                    </div>
                                </div>
                                <div class="m-b-10 f-left">
                                    <div dropdown class="btn-group">
                                        <button type="button" class="btn btn-warning">Action</button>
                                        <button type="button" dropdown-toggle class="btn btn-warning dropdown-toggle" data-toggle="dropdown">
                                            <span class="caret"></span>
                                            <span class="sr-only">Toggle Dropdown</span>
                                        </button>
                                        <span class="dropdown-arrow"></span>
                                        <ul class="dropdown-menu" role="menu">
                                            <li>
                                                <a href="#">Action</a>
                                            </li>
                                            <li>
                                                <a href="#">Another action</a>
                                            </li>
                                            <li>
                                                <a href="#">Something else here</a>
                                            </li>
                                            <li class="divider"></li>
                                            <li>
                                                <a href="#">Separated link</a>
                                            </li>
                                        </ul>
                                    </div>
                                </div>
                                <div class="m-b-10 f-left">
                                    <div dropdown class="btn-group">
                                        <button type="button" class="btn btn-primary">Action</button>
                                        <button dropdown-toggle type="button" class="btn btn-primary dropdown-toggle" data-toggle="dropdown">
                                            <span class="caret"></span>
                                            <span class="sr-only">Toggle Dropdown</span>
                                        </button>
                                        <span class="dropdown-arrow"></span>
                                        <ul class="dropdown-menu" role="menu">
                                            <li>
                                                <a href="#">Action</a>
                                            </li>
                                            <li>
                                                <a href="#">Another action</a>
                                            </li>
                                            <li>
                                                <a href="#">Something else here</a>
                                            </li>
                                            <li class="divider"></li>
                                            <li>
                                                <a href="#">Separated link</a>
                                            </li>
                                        </ul>
                                    </div>
                                </div>
                                <div class="m-b-10 f-left">
                                    <div dropdown class="btn-group">
                                        <button type="button" class="btn btn-dark">Action</button>
                                        <button dropdown-toggle type="button" class="btn btn-dark dropdown-toggle" data-toggle="dropdown">
                                            <span class="caret"></span>
                                            <span class="sr-only">Toggle Dropdown</span>
                                        </button>
                                        <span class="dropdown-arrow"></span>
                                        <ul class="dropdown-menu" role="menu">
                                            <li>
                                                <a href="#">Action</a>
                                            </li>
                                            <li>
                                                <a href="#">Another action</a>
                                            </li>
                                            <li>
                                                <a href="#">Something else here</a>
                                            </li>
                                            <li class="divider"></li>
                                            <li>
                                                <a href="#">Separated link</a>
                                            </li>
                                        </ul>
                                    </div>
                                </div>
                            </div>
                            <div class="col-md-4 clearfix">
                                <h3><strong>Inverse Dropdown Menu</strong> Look</h3>
                                <div class="m-b-10 f-left">
                                    <div dropdown class="btn-group">
                                        <button dropdown-toggle type="button" class="btn btn-dark dropdown-toggle" data-toggle="dropdown">
                                            Be Dark
                                            <span class="caret"></span>
                                        </button>
                                        <span class="dropdown-arrow dropdown-arrow-inverse"></span>
                                        <ul class="dropdown-menu dropdown-inverse" role="menu">
                                            <li>
                                                <a href="#">Action</a>
                                            </li>
                                            <li>
                                                <a href="#">Another action</a>
                                            </li>
                                            <li>
                                                <a href="#">Something else here</a>
                                            </li>
                                        </ul>
                                    </div>
                                </div>
                                <div class="m-b-10 f-left">
                                    <div dropdown class="btn-group">
                                        <button dropdown-toggle type="button" class="btn btn-white dropdown-toggle" data-toggle="dropdown">
                                            Be White
                                            <span class="caret"></span>
                                        </button>
                                        <span class="dropdown-arrow dropdown-arrow-inverse"></span>
                                        <ul class="dropdown-menu dropdown-inverse" role="menu">
                                            <li>
                                                <a href="#">Action</a>
                                            </li>
                                            <li>
                                                <a href="#">Another action</a>
                                            </li>
                                            <li>
                                                <a href="#">Something else here</a>
                                            </li>
                                        </ul>
                                    </div>

                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="footer">
            <div class="copyright">
                <p class="pull-left sm-pull-reset">
                    <span>Copyright <span class="copyright">&copy;</span> 2016 </span>
                    <span>THEMES LAB</span>.
                    <span>All rights reserved. </span>
                </p>
                <p class="pull-right sm-pull-reset">
                    <span><a href="#" class="m-r-10">Support</a> | <a href="#" class="m-l-10 m-r-10">Terms of use</a> | <a href="#" class="m-l-10">Privacy Policy</a></span>
                </p>
            </div>
        </div>
    </div>

</template>

<script>
    import MButtonGroup from '../components/button/ButtonGroup'
    import MButton from '../components/button/Button'

    export default {
        name: "ui-button",
        components:{MButton,MButtonGroup}
    }
</script>

<style scoped>

</style>
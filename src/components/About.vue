<template>
    <div class="about">
      <div class="container">
        <section class="section">
          <h1 class="title">About</h1>
        </section>
      </div>

      <div>
        <button id="show-modal" v-on:click="showModal = true">Show Modal</button>

        <modal v-if="showModal" v-on:close="showModal = false">
          <span slot="header">New header</span>
        </modal>
      </div>

      <hr/>
      <div><h1>BOOTSTRAP</h1></div>
      <div>https://www.w3schools.com/bootstrap4/default.asp</div>
      <div class="container">
        <h1>Class="container"</h1>
        <p>This part is inside a .container class.</p>
        <p>The .container class provides a responsive fixed width container.</p>
      </div>
      <br/>
      <div class="container-fluid">
        <h1>Class="container-fluid"</h1>
        <p>This is some text.</p>
      </div>

      <div>
        <p>col-sm-* columns will automatically stack on top of each other when the screen is greater than 576px wide.</p>
        <div class="row">
          <div class="col-sm-3" style="background-color:lavender;">.col-sm-3</div>
          <div class="col-sm-3" style="background-color:lavenderblush;">.col-sm-3</div>
          <div class="col-sm-3" style="background-color:lavender;">.col-sm-3</div>
          <div class="col-sm-3" style="background-color:lavenderblush;">.col-sm-3</div>
        </div>
      </div>

      <div>
        <p>col-md-* columns will automatically stack on top of each other when the screen is greater than 768px wide.</p>
        <div class="row">
          <div class="col-md-3" style="background-color:lavender;">.col-md-3</div>
          <div class="col-md-3" style="background-color:lavenderblush;">.col-md-3</div>
          <div class="col-md-3" style="background-color:lavender;">.col-md-3</div>
          <div class="col-md-3" style="background-color:lavenderblush;">.col-md-3</div>
        </div>
      </div>

      <div>
        <p>col-md-* columns will automatically stack on top of each other when the screen is greater than 768px wide.</p>
        <div class="row">
          <div class="col-lg-3" style="background-color:lavender;">.col-lg-3</div>
          <div class="col-lg-3" style="background-color:lavenderblush;">.col-lg-3</div>
          <div class="col-lg-3" style="background-color:lavender;">.col-lg-3</div>
          <div class="col-lg-3" style="background-color:lavenderblush;">.col-lg-3</div>
        </div>
      </div>

      <div>
        <p>col-xl-* columns will automatically stack on top of each other when the screen is greater than 1200px wide.</p>
        <div class="row">
          <div class="col-xl-3" style="background-color:lavender;">.col-xl-3</div>
          <div class="col-xl-3" style="background-color:lavenderblush;">.col-xl-3</div>
          <div class="col-xl-3" style="background-color:lavender;">.col-xl-3</div>
          <div class="col-xl-3" style="background-color:lavenderblush;">.col-xl-3</div>
        </div>
      </div>

      <div>
        <p>col- columns will automatically stack on top of each other when the screen is less than 576px wide.</p>
        <div class="row">
          <div class="col-" style="background-color:lavender;">.col-</div>
          <div class="col-" style="background-color:lavenderblush;">.col-</div>
          <div class="col-" style="background-color:lavender;">.col-</div>
          <div class="col-" style="background-color:lavenderblush;">.col-</div>
        </div>
      </div>

      <div class="container">
        <h1>h1 Bootstrap heading (2.5rem = 40px)</h1>
        <h2>h2 Bootstrap heading (2rem = 32px)</h2>
        <h3>h3 Bootstrap heading (1.75rem = 28px)</h3>
        <h4>h4 Bootstrap heading (1.5rem = 24px)</h4>
        <h5>h5 Bootstrap heading (1.25rem = 20px)</h5>
        <h6>h6 Bootstrap heading (1rem = 16px)</h6>
      </div>

      <div class="container">
        <h1>Display Headings</h1>
        <p>Display headings are used to stand out more than normal headings (larger font-size and lighter font-weight):</p>
        <h1 class="display-1">Display 1</h1>
        <h1 class="display-2">Display 2</h1>
        <h1 class="display-3">Display 3</h1>
        <h1 class="display-4">Display 4</h1>
      </div>

      <div class="container">
        <h2>Contextual Colors</h2>
        <p>Use the contextual classes to provide "meaning through colors":</p>
        <p class="text-muted">This text is muted.</p>
        <p class="text-primary">This text is important.</p>
        <p class="text-success">This text indicates success.</p>
        <p class="text-info">This text represents some information.</p>
        <p class="text-warning">This text represents a warning.</p>
        <p class="text-danger">This text represents danger.</p>
        <p class="text-secondary">Secondary text.</p>
        <p class="text-dark">This text is dark grey.</p>
        <p class="text-body">Default body color (often black).</p>
        <p class="text-light">This text is light grey (on white background).</p>
        <p class="text-white">This text is white (on white background).</p>
      </div>

      <div class="container">
        <h2>Contextual Link Colors</h2>
        <p>Hover over the links.</p>
        <a href="#" class="text-muted">Muted link.</a>
        <a href="#" class="text-primary">Primary link.</a>
        <a href="#" class="text-success">Success link.</a>
        <a href="#" class="text-info">Info link.</a>
        <a href="#" class="text-warning">Warning link.</a>
        <a href="#" class="text-danger">Danger link.</a>
        <a href="#" class="text-secondary">Secondary link.</a>
        <a href="#" class="text-dark">Dark grey link.</a>
        <a href="#" class="text-body">Body/black link.</a>
        <a href="#" class="text-light">Light grey link.</a>
      </div>

      <div class="container">
        <h2>Alerts</h2>
        <p>Alerts are created with the .alert class, followed by a contextual color classes:</p>
        <div class="alert alert-success">
          <strong>Success!</strong> This alert box could indicate a successful or positive action.
        </div>
        <div class="alert alert-info">
          <strong>Info!</strong> This alert box could indicate a neutral informative change or action.
        </div>
        <div class="alert alert-warning">
          <strong>Warning!</strong> This alert box could indicate a warning that might need attention.
        </div>
        <div class="alert alert-danger">
          <strong>Danger!</strong> This alert box could indicate a dangerous or potentially negative action.
        </div>
        <div class="alert alert-primary">
          <strong>Primary!</strong> Indicates an important action.
        </div>
        <div class="alert alert-secondary">
          <strong>Secondary!</strong> Indicates a slightly less important action.
        </div>
        <div class="alert alert-dark">
          <strong>Dark!</strong> Dark grey alert.
        </div>
        <div class="alert alert-light">
          <strong>Light!</strong> Light grey alert.
        </div>
      </div>

      <div class="container">
        <h2>Button Styles</h2>
        <button type="button" class="btn">Basic</button>
        <button type="button" class="btn btn-primary">Primary</button>
        <button type="button" class="btn btn-secondary">Secondary</button>
        <button type="button" class="btn btn-success">Success</button>
        <button type="button" class="btn btn-info">Info</button>
        <button type="button" class="btn btn-warning">Warning</button>
        <button type="button" class="btn btn-danger">Danger</button>
        <button type="button" class="btn btn-dark">Dark</button>
        <button type="button" class="btn btn-light">Light</button>
        <button type="button" class="btn btn-link">Link</button>
      </div>

      <div class="container">
        <h2>Button Elements</h2>
        <a href="#" class="btn btn-info" role="button">Link Button</a>
        <button type="button" class="btn btn-info">Button</button>
        <input type="button" class="btn btn-info" value="Input Button">
        <input type="submit" class="btn btn-info" value="Submit Button">
      </div>

      <div class="container">
        <h2>Button Group</h2>
        <p>The .btn-group class creates a button group:</p>
        <div class="btn-group">
          <button type="button" class="btn btn-primary">Apple</button>
          <button type="button" class="btn btn-primary">Samsung</button>
          <button type="button" class="btn btn-primary">Sony</button>
        </div>
      </div>

      <div class="container">
        <h2>Vertical Button Group</h2>
        <p>Use the .btn-group-vertical class to create a vertical button group:</p>
        <div class="btn-group-vertical">
          <button type="button" class="btn btn-primary">Apple</button>
          <button type="button" class="btn btn-primary">Samsung</button>
          <button type="button" class="btn btn-primary">Sony</button>
        </div>
      </div>

      <div class="container">
        <h2>Nesting Button Groups</h2>
        <p>Nest button groups to create dropdown menus:</p>
        <div class="btn-group">
          <button type="button" class="btn btn-primary">Apple</button>
          <button type="button" class="btn btn-primary">Samsung</button>
          <div class="btn-group">
            <button type="button" class="btn btn-primary dropdown-toggle" data-toggle="dropdown">
            Sony
            </button>
            <div class="dropdown-menu">
              <a class="dropdown-item" href="#">Tablet</a>
              <a class="dropdown-item" href="#">Smartphone</a>
            </div>
          </div>
        </div>
      </div>

      <div class="container">
        <h2>Progress Bar With Label</h2>
        <div class="progress">
          <div class="progress-bar" style="width:70%">70%</div>
        </div>
      </div>

      <div class="container">
        <h2>Pagination - Sizing</h2>
        <p>Add class .pagination-lg for larger blocks or .pagination-sm for smaller blocks.</p>

        <p>Large:</p>
        <ul class="pagination pagination-lg">
          <li class="page-item"><a class="page-link" href="#">Previous</a></li>
          <li class="page-item"><a class="page-link" href="#">1</a></li>
          <li class="page-item"><a class="page-link" href="#">2</a></li>
          <li class="page-item"><a class="page-link" href="#">3</a></li>
          <li class="page-item"><a class="page-link" href="#">Next</a></li>
        </ul>

        <p>Default:</p>
        <ul class="pagination">
          <li class="page-item"><a class="page-link" href="#">Previous</a></li>
          <li class="page-item"><a class="page-link" href="#">1</a></li>
          <li class="page-item"><a class="page-link" href="#">2</a></li>
          <li class="page-item"><a class="page-link" href="#">3</a></li>
          <li class="page-item"><a class="page-link" href="#">Next</a></li>
        </ul>

        <p>Small:</p>
        <ul class="pagination pagination-sm">
          <li class="page-item"><a class="page-link" href="#">Previous</a></li>
          <li class="page-item"><a class="page-link" href="#">1</a></li>
          <li class="page-item"><a class="page-link" href="#">2</a></li>
          <li class="page-item"><a class="page-link" href="#">3</a></li>
          <li class="page-item"><a class="page-link" href="#">Next</a></li>
        </ul>
      </div>

      <div class="container">
        <h2>List Group With Contextual Classes</h2>
        <ul class="list-group">
          <li class="list-group-item list-group-item-success">Success item</li>
          <li class="list-group-item list-group-item-secondary">Secondary item</li>
          <li class="list-group-item list-group-item-info">Info item</li>
          <li class="list-group-item list-group-item-warning">Warning item</li>
          <li class="list-group-item list-group-item-danger">Danger item</li>
          <li class="list-group-item list-group-item-primary">Primary item</li>
          <li class="list-group-item list-group-item-dark">Dark item</li>
          <li class="list-group-item list-group-item-light">Light item</li>
        </ul>
      </div>

      <div class="container">
        <h2>Card Deck</h2>
        <p>The .card-deck class creates an <strong>equal height and width</strong> grid of cards. The layout will automatically adjust as you insert more cards.</p>
        <p>In this example we have added extra content to the first card, to make it taller. Notice how the other cards follow.</p>
        <p><strong>Note:</strong> The cards are displayed vertically on small screens (less than 576px):</p>
        <div class="card-deck">
          <div class="card bg-primary">
            <div class="card-body text-center">
              <p class="card-text">Some text inside the first card</p>
              <p class="card-text">Some more text to increase the height</p>
              <p class="card-text">Some more text to increase the height</p>
              <p class="card-text">Some more text to increase the height</p>
            </div>
          </div>
          <div class="card bg-warning">
            <div class="card-body text-center">
              <p class="card-text">Some text inside the second card</p>
            </div>
          </div>
          <div class="card bg-success">
            <div class="card-body text-center">
              <p class="card-text">Some text inside the third card</p>
            </div>
          </div>
          <div class="card bg-danger">
            <div class="card-body text-center">
              <p class="card-text">Some text inside the fourth card</p>
            </div>
          </div>
        </div>
      </div>

      <div class="container">
        <h2>Dropdowns</h2>
        <p>The .dropdown-divider class is used to separate links inside the dropdown menu with a thin horizontal line:</p>
        <div class="dropdown">
          <button type="button" class="btn btn-primary dropdown-toggle" data-toggle="dropdown">
            Dropdown button
          </button>
          <div class="dropdown-menu">
            <a class="dropdown-item" href="#">Link 1</a>
            <a class="dropdown-item" href="#">Link 2</a>
            <a class="dropdown-item" href="#">Link 3</a>
            <div class="dropdown-divider"></div>
            <a class="dropdown-item" href="#">Another link</a>
          </div>
        </div>
      </div>

      <div class="container">
        <h2>Modal Example</h2>
        <!-- Button to Open the Modal -->
        <button type="button" class="btn btn-primary" data-toggle="modal" data-target="#myModal">
          Open modal
        </button>

        <!-- The Modal -->
        <div class="modal" id="myModal">
          <div class="modal-dialog">
            <div class="modal-content">

              <!-- Modal Header -->
              <div class="modal-header">
                <h4 class="modal-title">Modal Heading</h4>
                <button type="button" class="close" data-dismiss="modal">&times;</button>
              </div>

              <!-- Modal body -->
              <div class="modal-body">
                Modal body..
              </div>

              <!-- Modal footer -->
              <div class="modal-footer">
                <button type="button" class="btn btn-danger" data-dismiss="modal">Close</button>
              </div>

            </div>
          </div>
        </div>
      </div>

      <hr/>
      HTML5 Graphics
      <div>canvas, svg</div>
      SVG
      <svg width="100" height="100">
        <circle cx="50" cy="50" r="40" stroke="green" stroke-width="4" fill="yellow" />
        Sorry, your browser does not support inline SVG.
      </svg>

      <svg width="400" height="180">
        <rect x="50" y="20" rx="20" ry="20" width="150" height="150" style="fill:red;stroke:black;stroke-width:5;opacity:0.5" />
        Sorry, your browser does not support inline SVG.
      </svg>

      <svg width="300" height="200">
        <polygon points="100,10 40,198 190,78 10,78 160,198"
        style="fill:lime;stroke:purple;stroke-width:5;fill-rule:evenodd;" />
      </svg>

      <svg height="130" width="500">
        <defs>
        <linearGradient id="grad1" x1="0%" y1="0%" x2="100%" y2="0%">
          <stop offset="0%" style="stop-color:rgb(255,255,0);stop-opacity:1" />
          <stop offset="100%" style="stop-color:rgb(255,0,0);stop-opacity:1" />
        </linearGradient>
        </defs>

        <ellipse cx="100" cy="70" rx="85" ry="55" fill="url(#grad1)" />

        <text fill="#ffffff" font-size="45" font-family="Verdana" x="50" y="86">SVG</text>
      </svg>

      <hr/>
      HTML5 New Media Elements
      <div>audio, embed, source, track, video</div>
      AUDIO
      <audio controls>
        <source src="https://www.w3schools.com/tags/horse.ogg" type="audio/ogg">
        <source src="https://www.w3schools.com/tags/horse.mp3" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio>

      VIDEO
      <video width="320" height="240" controls>
        <source src="https://www.w3schools.com/tags/movie.mp4" type="video/mp4">
        <source src="https://www.w3schools.com/tags/movie.ogg" type="video/ogg">
        Your browser does not support the video tag.
      </video>

      <hr/>
      New Semantic Elements in HTML5
      <div>article, aside, details, figcation, figure, footer, header, main,
        mark nav,section, summary, time</div>

      <div>Nav</div>
      <nav>
        <a href="/html/">HTML</a> |
        <a href="/css/">CSS</a> |
        <a href="/js/">JavaScript</a> |
        <a href="/jquery/">jQuery</a>
      </nav>

      <hr/>

    </div>
</template>

<!-- check work code on pulling in import -->
<script>
import modal from '@/components/Modal'
export default {
  name: 'about',
  template: {
    modal
  },
  data:  () => ({
    showModal: false
  })
}
</script>

<style lang="sass" scoped>
@import '../mq'

.about
  padding: 2.4em;

.pd
  padding: 2.4em 0 1.5em 0

.answer
  margin-top: 10px !important
  color: gray

.columns
  flex-wrap: wrap

</style>

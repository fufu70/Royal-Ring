# Royal Ring
A SASS mix that creates a responsive ring inside of a ring with content contained inside of the center ring.

## Installation

To add the project with bower simply run:

```shell
$ bower install 'git://github.com/fufu70/Royal-Ring.git'
```

## Usage

Once the repo has been installed you can import the `royal-ring` file into your respective sass file with a specific namespace:

```sass
@import "path/to/royal-ring";

.hero-unit {
    @include royal-ring(
        160px,   /* size */
        #ffff66, /* background-start */
        #ffcc00, /* background-stop */
        #7a0099, /* circle-background-start */
        #9432ad, /* circle-background-mid */
        #7a0099, /* circle-background-stop */
        70%,     /* circle-percentage-stop */
        42px,    /* font-size */
        #ffffff, /* font-color */
        #ffff66, /* breaker-start-color */
        #ffcc00  /* breaker-end-color */
    );
}
```

The variables above are the default variables for the `@mixin`.

The html structure is as follows: 

```html
<div class="hero-unit">
    <div class="hero-unit__counter hero-unit__ring-start">
        <div class="hero-unit__counter__outer-ring">
            <div class="hero-unit__ring-start hero-unit__ring-start-inner">
                <div class="hero-unit__counter__inner-ring">
                    <div class="hero-unit__ring-contents">
                        <div class="hero-unit__ring-contents__counter ng-binding">3</div>
                        <div class="hero-unit__ring-contents__breaker">
                            <div class="hero-unit__ring-contents__breaker__line">
                                <div class="hero-unit__ring-contents__breaker__triangle"></div>
                            </div>
                            <div class="hero-unit__ring-contents__breaker__glow-container">
                                <div class="hero-unit__ring-contents__breaker__glow"></div>
                            </div>
                        </div>
                        <div class="hero-unit__ring-contents__description">HERO UNITS</div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>
```

![alt text][example]

## Testing

To test the repository clone the repo, install gulp and bower globally, install npm packages, install bower packages, and run the gulp server:

```shell
$ git clone https://github.com/fufu70/Royal-Ring
$ cd Unordered-List-Linker
$ npm install --global gulp-cli bower
$ npm install
$ bower install
$ gulp serve
```

[example]: https://raw.githubusercontent.com/fufu70/Royal-Ring/master/common/example.png "Example"

## Authors
* [Anthony Delaura](http://www.anthonydelaura.com/) - Designed the Ring.
* [Christian Micklisch](https://github.com/fufu70) - CSS styling.
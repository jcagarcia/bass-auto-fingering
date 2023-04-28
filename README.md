# Double Bass Fingering Ruby Gem

The Double Bass Fingering Ruby Gem is a tool designed for bassists who want to maximize the efficiency of their fingering positions when playing the double bass. This gem provides automatic calculation of the best fingering positions based on a given set of notes.

## Features

* Automatic calculation of the most efficient fingering positions based on a list of notes.

## Installation

The Double Bass Fingering Ruby Gem can be installed via RubyGems:

```sh
gem install double_bass_fingering
```

## Usage

To use the Double Bass Fingering Ruby Gem, simply require it in your Ruby code:

```ruby
require 'double_bass_fingering'
```

Then, perform the `AutoFingering::DoubleBass.calculate_for` method passing the array of notes you need to play:

```ruby
fingering = DoubleBassFingering.calculate_for(["C1", "D1", "E1", "F1", "G1", "A1", "B1", "C2"]) # => [2, 0, 1, 2, 0, 1, 2, 4]
```

The calculate_for method returns an array of integers representing the finger positions for each string. A 0 value indicates an open string, and a positive integer indicates the fret position.

## Contributing

Contributions are welcome! If you would like to contribute to the Double Bass Fingering Ruby Gem, please fork this repository and submit a pull request.

## License

The Double Bass Fingering Ruby Gem is released under the Apache 2.0 License.

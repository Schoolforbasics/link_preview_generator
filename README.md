# LinkPreviewGenerator

LinkPreviewGenerator is a package that tries to receive meta information from given http(s) address

## Installation

If [available in Hex](https://hex.pm/docs/publish), the package can be installed as:

  1. Add link_preview_generator to your list of dependencies in `mix.exs`:

        def deps do
          [{:link_preview_generator, "~> 0.0.1"}]
        end

  2. Ensure link_preview_generator is started before your application:

        def application do
          [applications: [:link_preview_generator]]
        end

## Example usage

You just need to execute:

    LinkPreviewGenerator.parse("www.yahoo.pl")

in response you'll receive

    %LinkPreviewGenerator.Page{description: "News, email and search are just the beginning. Discover more every day. Find your yodel.",
      images: [%{url: "https://s.yimg.com/dh/ap/default/130909/y_200_a.png"}],
      original_url: "yahoo.pl", title: "Yahoo", website_url: "https://www.yahoo.com"}

## License

  Copyright [2016] [Tobiasz Małecki <tobiasz.malecki@appunite.com>]

  Licensed under the Apache License, Version 2.0 (the "License");
  you may not use this file except in compliance with the License.
  You may obtain a copy of the License at

	http://www.apache.org/licenses/LICENSE-2.0


  Unless required by applicable law or agreed to in writing, software
  distributed under the License is distributed on an "AS IS" BASIS,
  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  See the License for the specific language governing permissions and
  limitations under the License.

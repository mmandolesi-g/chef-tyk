tyk Cookbook
============

Install and configure Tyk API gateway (https://tyk.io)

## Usage

- For a testing installation, just add the `tyk::default` recipe to your 
runlist. It will install Redis, Mongo, Tyk Gateway and Tyk Dashboard on the
node. You have to bootstrap the dashboard with an initial user, as per manual.
After that, point your browser to your node port 3000 and the dashboard
should come up and let you login with the user you created during the
bootstrap.
- For production, use the provided `install_gateway` and `install_dashboard`
recipes. You will want to change the configuration attributes. Best solution
is to create your own wrapper cookbook, where you set the `default` attributes.

## Contributing

1. Fork the repository on Github
2. Create a named feature branch (like `add_component_x`)
3. Write your change
4. Write tests for your change (if applicable)
5. Run the tests, ensuring they all pass
6. Submit a Pull Request using Github

## License and Author

  * Author: Michal Taborsky <michal@taborsky.cz>

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0`

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.
#
# Copyright 2015, Noah Kantrowitz
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
# http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
#

source 'https://supermarket.chef.io/'
extension 'halite'

# Force the rebuild every time for development.
cookbook 'poise', gem: 'poise'
cookbook 'application', gem: 'poise-application'

group :test do
  cookbook 'application_test', path: 'test/cookbooks/application_test'
  cookbook 'apt'
end
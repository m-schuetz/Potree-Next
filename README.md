# About

Potree is an Open Source viewer for massive point cloud data sets, capable of displaying data sets with billions of points in web browsers. 

Potree-Next is a rewrite of [Potree](https://github.com/potree/potree/) in WebGPU. WebGPU is the upcoming succesor of WebGL, providing a more modern graphics API and features such as compute shaders. With Potree-Next, we want to take advantage of these new features and rebuild Potree from scratch, getting rid of legacy baggage that accumulated over 13 years and doings things right.

This effort is funded by [Netidee](https://www.netidee.at/) and also has new capabilities in mind:
* Support for 3D-Tiles
* Support for arbitrary point attributes
* A new point cloud file format
* Support for Gaussian Splats

A rewrite evidently has the disadvantage that many features that are currently present in Potree will initially be missing, but we will start out with other, new ones that Potree does not have. By the time WebGPU is widely supported in all browsers and devices -- including Linux and mobile devices --  we plan to catch up with most functionality.

# Examples

<table>
	<tr>
		<td><a href="https://users.cg.tuwien.ac.at/mschuetz/permanent/potree-next/3dtiles.html"><img src="./docs/3DTiles.jpg"/></a></td>
		<td><a href="https://users.cg.tuwien.ac.at/mschuetz/permanent/potree-next/vienna_city_center.html"><img src="./docs/vienna.jpg"/></a></td>
		<td><a href="https://users.cg.tuwien.ac.at/mschuetz/permanent/potree-next/gaussians.html"><img src="./docs/points_n_splats.jpg"/></a></td>
		<td><a href="https://users.cg.tuwien.ac.at/mschuetz/permanent/potree-next/extra_materials_terrasolid_sitn.html"><img src="./docs/extra_attributes.jpg"/></a></td>
	</tr>
	<tr>
		<th>3D Tiles</th>
		<th>Vienna Inner City</th>
		<th>Points and Splats</th>
		<th>Extra Attributes</th>
	</tr>
</table>




# Getting Started

* Convert your point cloud with [PotreeConverter](https://github.com/potree/PotreeConverter) or [PotreeDesktop](https://github.com/potree/potreedesktop).
* Clone or download this repository.
* Copy and adapt one of the examples, e.g., lion.html.
* Run it in your web browser to see the results.
	* To run it on your local machine, you can install [node.js](https://nodejs.org/en)
	* Then install the "http-server" package system-wide (-g): <br>
	  ```npm install -g http-server```
	* Run the server from within the Potree-Next directory: <br>```http-server```
	* Open one of the examples in your web browser, e.g.: <br>
	  ```http://localhost:8080/lion.html```
* Once it works locally, you can upload the results to your file server to make it accessible online. Potree is a client-side renderer, so a simple file server without PHP, JS, etc. is sufficient. 

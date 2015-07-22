# react-safe-render
Helper to make sure your react components do not kill your entire Application when they fail to render

## Usage Example

		var ReactSafeRender = require('react-safe-render');

		// Optionally provide an error handler
		var safeRenderConfig = {
			errorHandler: function(info) {
				console.error("Error in component", info.displayName, info.error);
			}
		};

		ReactSafeRender(React, safeRenderConfig);

# docs.flyyer.io

> CSS Theme: https://facebookincubator.github.io/infima/

This website is built using [Docusaurus 2](https://v2.docusaurus.io/), a modern static website generator.

## Installation

```console
yarn install
```

## Local Development

```console
yarn start
```

This command starts a local development server and open up a browser window. Most changes are reflected live without having to restart the server.

### Using remote files

To avoid copy-paste going out of sync with different projects you can use this MDX component to render remote files:

```jsx
export const RemoteFile = ({children, source, ...props}) => {
  const [code, setCode] = React.useState(null);
  const [error, setError] = React.useState(null);
  React.useEffect(() => {
    fetch(source)
      .then((res) => {
        if (res.ok) {
          res.text().then(text => setCode(text));
        } else {
          res.text().then(err => setError(new Error(err)));
        }
      })
      .catch(err => setError(err));
  }, [source]);
  return (
    <code {...props}>
      {code || "Loading..."}
    </code>
  )
};

<RemoteFile source="https://raw.githubusercontent.com/useflyyer/flyyer-actions/main/workflow-templates/flyyer-yarn.yml" />
```

## Build

```console
yarn build
```

This command generates static content into the `build` directory and can be served using any static contents hosting service.

## Deployment

Just push to `main`. We are using Vercel to deploy.

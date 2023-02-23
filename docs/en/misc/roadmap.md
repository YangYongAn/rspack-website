# Roadmap

While we do expect to support the features listed below in the future, we do not guarantee that all of the features listed below will be supported, in the next release, if at all. Additionally we do not guarantee that they will be implemented in the order listed below.

### Performance Improvement

### Support for more community plugins and loaders

As webpack contains a large number of apis, we will be working to support the most frequently used loaders and plugins based on feedback from the community first.

### Module Federation support

Module Federation is a widely used webpack feature with a rich ecosystem and we will be working with the author of Module Federation [Zack Jackson](https://github.com/ScriptedAlchemy) together with the Module Federation core team and their product owner @viktoriialurie, to develop support for module federation.

### Vue and Svelte support

From what we have seen, Vue and Svelte are two very popular front-end frameworks that are more complex to support than React. They rely on more internal webpack apis. We expect to complete full support for both frameworks in the near future. Our desire is to support the full Vue and Svelte ecosystems.

### Lazy Compilation support

Although Rspack currently has good performance, there is still a lot of room to improve performance for projects with a large number of pages, and Lazy Compilation is a good way to improve performance.
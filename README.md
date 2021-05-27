# fetily

```
import { createFetily } from 'fetily';

interface API {
	hello: {
		get({
			username: string
		}): Promise<{
			world: string;
		}>;
	};
	'dog/fish-hello': {
		get({
			aa: string
		}): Promise<{
			data: { name: string; age: number }[];
		}>;
	};
}

export const fetily = createFetily<API>({ baseUrl: '/api' });

```

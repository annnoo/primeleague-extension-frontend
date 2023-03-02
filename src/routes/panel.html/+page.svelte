<script>
	const i = [100, 200, 300];

	const tableArr = [
		{
			position: '1',
			name: 'NNO Prime',
			img: 'https://cdn0.gamesports.net/edb_team_logos_light/29000/29951.png',
			symbol: '12 - 0',
		},
	{
			position: '1',
			name: 'NNO Prime',
			img: 'https://cdn0.gamesports.net/edb_team_logos_light/29000/29951.png',
			symbol: '12 - 0',
		}
	];
</script>

<div class="h-screen w-screen  bg-gray-900">
	<div class="overflow-x-auto w-full bg-gray-900 p-4 border-gray-800">
		<table class=" w-full text-sm text-left text-gray-500 dark:text-gray-400 h-full">
			<thead class="bg-black text-sm text-gray-200 uppercase  border-b border-gray-700">
				<tr class="">
					<th class="p-3">#</th>
					<th>Team</th>
					<th>W-L</th>
				</tr>
			</thead>
			<tbody class="bg-neutral-800 text-white">
				{#each tableArr as row, i}
					<tr class="m-2 border-b border-gray-700 ">
						<td class="m-2 p-2">{row.position}.</td>
						<td>
							<a
								class="flex flex-row align-top text-center items-center w-full h-full font-sans text-xs font-normal  text-white cursor-pointer hover:text-cyan-300"
								href="https://www.primeleague.gg/teams/21801-unicorns-of-love-sexy-edition"
                target="_blank"
								style="outline: 0px; text-decoration: none; transition: color 100ms ease-in-out 0s;"
							>
								<img
									alt="Unicorns of Love Sexy Edition"
									src="{row.img}"
									data-loaded="true"
									class="w-6 max-w-full "
									style="outline: 0px; transition: filter 150ms ease-in-out 0s;"
								/>

								<span class="text-center ml-2 align-middle " style=""
									>{row.name}</span
								>
							</a>
						</td>
						<td>{row.symbol}</td>
					</tr>
				{/each}
			</tbody>
        <tfoot>
        <tr  class="bg-black">
          <td colspan="3" class="text-center p-2 w-full">

            <div class="text-center flex flex-row items-center justify-center">
              <a href="https://www.primeleague.gg/" target="_blank"> 
                <img class="w-24 text-center" src="https://cdn1-v3.gamesports.net/img/themes/primeleague/logo_prm_strauss.svg?1"/>

              </a>
            </div>
          </td>
        </tr>
      </tfoot>
		</table>
	</div>
</div>
